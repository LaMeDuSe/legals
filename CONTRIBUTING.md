# Guide d'édition des documents juridiques — LaMeDuSe

*CONTRIBUTING.md — processus de modification des textes contractuels du dépôt*

---

## 1. Structure du dépôt

| Emplacement | Rôle |
|---|---|
| `src/*.md` | Sources des documents contractuels (CGV, CGP, annexes, conditions particulières) |
| `refs/*.json` | Métadonnées de chaque document : `name`, `last_updated`, `version`, `src`, `description` |
| `alls.json` | Index ordonné de tous les fichiers `refs/` |
| `CONTRIBUTING.md` | Le présent guide (non contractuel, jamais référencé dans `alls.json`) |

## 2. Règle de versionnement — un commit = une nouvelle version

**Tout commit qui modifie le contenu d'un document contractuel entraîne la création d'une nouvelle version de ce document.** La version et la date sont systématiquement incrémentées à chaque édition, même mineure.

Pour chaque document modifié :

1. **Bump de la version** dans `refs/<document>.json` : `"version"` est incrémentée de 1 (ex. `"3"` → `"4"`). Un nouveau document démarre en version `"1"`.
2. **Mise à jour de la date** dans `refs/<document>.json` : `"last_updated"` prend la date du jour au format ISO `AAAA-MM-JJ` (ex. `2026-11-06`).
3. **Mise à jour du pied de page** du fichier `src/<document>.md` : `*Dernière mise à jour : <jour> <mois en toutes lettres> <année>*` (ex. `6 novembre 2026`).

Si un même commit modifie plusieurs documents, **chaque document concerné est bumpé individuellement** (version et date).

La date reste identique si plusieurs éditions ont lieu le même jour ; seule la version matérialise le nombre d'éditions.

## 3. Processus d'édition d'un article

1. Identifier le ou les documents concernés et vérifier les renvois croisés (ex. `grep -n "article X" src/*.md`).
2. Éditer le fichier `src/` en respectant le style :
   - titre principal `#`, articles `## Article N : Titre`, sous-sections numérotées `N.M.` (pas de titres `###` pour les subdivisions courantes) ;
   - listes à puces pour les énumérations, listes indentées pour les subdivisions d'un même alinéa ;
   - texte juridique en français, gras `**...**` pour les notions clés et montants ;
   - séparation des articles par `---` et lignes vides simples (pas de doubles lignes vides).
3. Si la modification renumérote des articles ou sous-articles, **mettre à jour tous les renvois internes** dans tous les documents du dépôt.
4. Bumper version et date conformément à la section 2.
5. Vérifier avant commit :
   - validité JSON de `alls.json` et des `refs/` modifiés (`python -c "import json; json.load(open('...'))"`) ;
   - cohérence de la numérotation (articles et sous-articles continus) ;
   - absence de doublons dans `alls.json` ;
   - présence du pied de page SIREN et de la date à jour.

## 4. Conventions de commit

Format recommandé :

```
docs(<document>): <description de la modification>
```

Exemples :

```
docs(license-cgv): encadrement de la décompilation (notification 8 jours, demande préalable)
docs(payments-terms): clause penale sur les frais administratifs (art. 7.5)
docs(cloud-cgv-gen): restriction aux professionnels (art. 2, 10, 32)
```

Un commit contenant une modification de contenu **doit** inclure le bump de version/date correspondant dans le même commit.

## 5. Ajout d'un nouveau document

1. Créer `src/<nom>.md` (version 1, date du jour, pied de page SIREN).
2. Créer `refs/<nom>.json` avec `name`, `last_updated`, `version: "1"`, `src`, `description`.
3. Ajouter la référence dans `alls.json` à l'emplacement logique (ordre thématique : CGV générales, CGP, conditions particulières, annexes, mentions).
4. Vérifier les renvois croisés depuis les documents existants.

## 6. Hiérarchie contractuelle de référence

Lors de toute rédaction, rappeler l'ordre de priorité entre documents (exemple CGV-L art. 18.1) : devis signé → conditions particulières / contrats spécifiques → CGV du domaine → CGV générales → CGP (prévalent pour les modalités et pénalités de paiement).

## 7. Clause d'indépendance des stipulations (divisibilité)

### 7.1 Règle

Toute **clause d'indépendance des stipulations** (nullité partielle / divisibilité) est **obligatoire** dans tout document contractuel autonome (CGV, CGP, DPA, conditions de licence, tout contrat général). Elle est ajoutée dans les dispositions finales ou diverses du document.

Toute création de nouveau document autonome doit inclure cette clause ; toute modification ou déplacement de la clause suit le processus de versionnement de la section 2 (bump de version et de date).

### 7.2 Formulation standard

> **Indépendance des stipulations** : si l'une des clauses des présentes venait à être déclarée nulle ou inapplicable, les autres stipulations demeureraient pleinement en vigueur ; les Parties s'efforceraient de bonne foi de négocier une clause de remplacement de portée équivalente.

### 7.3 Localisation actuelle de la clause

| Document | Article |
|---|---|
| CGV Cloud (`src/lameduse-cloud-cgv-gen.md`) | Art. 37.1 « Nullité partielle » |
| CGV Forfaits (`src/lameduse-retainers.md`) | Art. 31 |
| CGP (`src/lameduse-payments-terms.md`) | Art. 10.4 « Indépendance des stipulations » |
| CGV Développement Logiciel (`src/lameduse-dev-cgv.md`) | Art. 21.4 « Indépendance des stipulations » |
| CGV-L Artémis & MedEyes (`src/lameduse-license-cgv.md`) | Art. 18.4 « Indépendance des stipulations » |
| CGV Design (`src/lameduse-design-cgv.md`) | Art. 14.4 « Indépendance des stipulations » |
| CGV Intelligence Artificielle (`src/lameduse-ai-cgv.md`) | Art. 14.4 « Indépendance des stipulations » |
| DPA (`src/lameduse-dpa.md`) | Art. 12 « Indépendance des stipulations » |

### 7.4 Documents exemptés (héritage ou non-contractuel)

- **Annexes : Conditions Particulières (7 CP), AUP, annexe SLA, liste des sous-traitants** — ces documents font partie intégrante de leur document parent (CGV Cloud, CGV Forfaits ou DPA) et **héritent de plein droit** de sa clause d'indépendance. Ne pas la dupliquer, sauf décision contraire documentée dans le commit.
- **Documents d'information non contractuels** : `mentions-legales.md`, `politique-confidentialite.md` — une clause de divisibilité n'y a pas d'objet.

### 7.5 Contrôle de couverture

Vérification périodique (lors de toute revue du dépôt) :

```bash
for f in src/*.md; do
  r=$(grep -ic "nulle ou inapplicable\|conserveraient toute leur force\|demeureraient pleinement" "$f")
  echo "$f : $r"
done
```

Un document contractuel autonome affichant `0` doit être corrigé (ajout de la clause + bump de version/date) dans le commit correspondant.

---

*Guide interne d'édition — LaMeDuSe SAS. Dernière mise à jour : 6 novembre 2026.*
