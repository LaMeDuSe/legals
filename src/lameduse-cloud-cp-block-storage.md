# Conditions Particulières : Service de Disque Réseau (Stockage Bloc)

**LaMeDuSe SAS**

---

## Préambule

Les présentes Conditions Particulières (ci-après les « **CP** ») complètent et précisent les Conditions Générales de Vente Services d'Hébergement de LaMeDuSe SAS (ci-après les « **CGV** ») pour ce qui concerne spécifiquement le service de **disque réseau**, ou stockage bloc, rattaché à une instance de calcul (ci-après le « **Service** »).

Conformément à l'article 37.3 des CGV, en cas de contradiction entre les documents contractuels, l'ordre de priorité suivant s'applique : (i) le Devis ou Bon de Commande, (ii) les présentes CP, (iii) les CGV, (iv) les autres annexes. Pour tout point non traité par les présentes CP, les dispositions des CGV s'appliquent pleinement.

---

## Article 1 : Objet

Les présentes CP ont pour objet de définir les conditions spécifiques applicables à la fourniture par LaMeDuSe d'un ou plusieurs volumes de stockage bloc (disques réseau) rattachables à un serveur virtuel (VPS), un serveur dédié ou une autre instance de calcul du Client, dans les conditions décrites au Devis.

---

## Article 2 : Définitions spécifiques

- **Disque réseau (volume bloc)** : espace de stockage présenté au Client sous forme de volume bloc, rattachable à une instance de calcul comme un disque, accessible via le réseau interne de LaMeDuSe.
- **Rattachement (attachement)** : opération consistant à associer un volume à une instance de calcul déterminée, à laquelle il devient accessible.
- **IOPS / débit** : indicateurs de performance du volume (opérations d'entrée/sortie par seconde, débit) précisés au Devis selon le type de volume souscrit.
- **Instance de rattachement** : serveur virtuel, serveur dédié ou autre ressource de calcul du Client à laquelle le volume est rattaché.

---

## Article 3 : Description du Service et localisation

3.1. Le Service met à disposition du Client un ou plusieurs volumes de stockage bloc, dont la capacité, le type (par exemple SSD ou autre) et les performances (IOPS, débit) sont précisés au Devis.

3.2. Un volume est rattaché à une instance de calcul située dans le même Datacenter et la même zone que le volume. Le volume n'est pas accessible indépendamment d'une instance de rattachement.

3.3. Le niveau de redondance du volume au sein de la plateforme est celui précisé au Devis. Cette redondance ne constitue pas une sauvegarde au sens de l'article 5 des présentes CP.

3.4. Le volume est hébergé dans un Datacenter situé en **France, en Allemagne ou en Suisse**, la localisation retenue étant indiquée au Devis, conformément à l'article 4 des CGV.

---

## Article 4 : Commande, mise à disposition et redimensionnement

4.1. Toute commande fait l'objet d'un Devis précisant la capacité, le type de volume, les performances et le tarif applicable.

4.2. Le volume est provisionné de manière automatisée et rendu disponible au rattachement depuis l'interface de gestion du Client.

4.3. Le Client peut, selon les options disponibles au Devis, augmenter la capacité d'un volume. Toute opération de redimensionnement relève de la responsabilité du Client s'agissant de l'adaptation du système de fichiers correspondant.

---

## Article 5 : Sauvegarde et snapshots

5.1. Sauf option de sauvegarde ou de snapshots souscrite au Devis, LaMeDuSe n'assure aucune sauvegarde des données présentes sur le volume. La redondance interne éventuellement incluse ne protège pas contre une suppression, une corruption ou une altération des données par le Client ou ses applications, et ne constitue pas une sauvegarde.

5.2. Il appartient au Client de mettre en œuvre sa propre politique de sauvegarde. Lorsqu'une option de sauvegarde ou de snapshots est souscrite, ses modalités (fréquence, durée de rétention, procédure de restauration) sont précisées au Devis.

---

## Article 6 : Niveau de service (SLA)

6.1. LaMeDuSe garantit, pour l'infrastructure de stockage relevant de sa responsabilité, un taux de disponibilité mensuel qui dépend de la **gamme de service** souscrite et précisée au Devis (**99,9 %** pour la gamme Essentiel, **99,95 %** pour la gamme Avancé, **99,99 %** pour la gamme Critique), mesuré sur une base mensuelle glissante, dans les conditions et exclusions prévues à l'article 12 des CGV et à l'annexe SLA. À défaut d'indication de gamme au Devis, la gamme Essentiel (99,9 %) s'applique.

6.2. Ce SLA porte sur la disponibilité du volume et de son accessibilité réseau au sein de l'infrastructure de LaMeDuSe. Il ne couvre pas les indisponibilités résultant de l'instance de rattachement, du système d'exploitation, des systèmes de fichiers, des configurations ou des manipulations du Client.

---

## Article 7 : Responsabilités du Client

7.1. Le Client est seul responsable :
   - de la configuration, du formatage et de la gestion du système de fichiers du volume ;
   - de la cohérence des données lors des opérations de rattachement, de détachement et de redimensionnement ;
   - de la sauvegarde de ses données, sauf option souscrite au Devis ;
   - de l'usage conforme du Service au regard de la réglementation applicable et de l'AUP prévue à l'article 14 des CGV.

7.2. Le Client garantit LaMeDuSe contre toute conséquence dommageable résultant d'un contenu illicite stocké sur le volume dont il a la charge.

---

## Article 8 : Suspension et résiliation

8.1. En cas de manquement du Client à ses obligations (impayé, usage abusif, contenu illicite, signalement d'abus non traité), LaMeDuSe applique les modalités de suspension prévues aux articles 14.4 et 18 des CGV et à l'AUP.

8.2. La résiliation du Service par le Client s'effectue avec un préavis de **trente (30) jours calendaires** avant la fin de la période de facturation en cours, sauf disposition contraire au Devis.

---

## Article 9 : Sort des données en fin de contrat

9.1. Il appartient au Client d'avoir réalisé, avant la date d'effet de la résiliation ou de l'expiration du Service, l'ensemble des sauvegardes et exports des données présentes sur le volume. À la date d'effet de la résiliation, l'accès au volume est coupé.

9.2. La restitution et la suppression des Données s'effectuent dans les conditions de réversibilité de l'article 9 des CGV, la période de conservation de **trente (30) jours** prévue à l'article 9.2 des CGV s'appliquant, sauf disposition contraire au Devis. Passé ce délai, le volume est effacé de manière sécurisée et remis en disponibilité.

---

## Article 10 : Obligation légale d'identification (LCEN)

Conformément au V de l'article 6 de la loi n° 2004-575 du 21 juin 2004 pour la confiance dans l'économie numérique (LCEN), dans sa rédaction issue de la loi n° 2024-449 du 21 mai 2024, et à l'article L. 34-1 du Code des postes et des communications électroniques, LaMeDuSe, en sa qualité de fournisseur de services d'hébergement, détient et conserve les données de nature à permettre l'identification des contributeurs aux contenus, dans les conditions de l'article 19 des CGV. Le Client s'engage à fournir des informations d'identification exactes et à jour, conformément à l'article 6 des CGV.

---

## Article 11 : Articulation avec les CGV

Pour tout point non expressément traité par les présentes CP (facturation, responsabilité, données personnelles, force majeure, résiliation pour manquement, droit applicable, juridiction compétente), les dispositions des CGV Hébergement LaMeDuSe s'appliquent pleinement et sans réserve.

---

*Dernière mise à jour : 16 juillet 2026*
