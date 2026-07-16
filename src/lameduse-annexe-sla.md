# Annexe SLA : Niveaux de Service et Barème de Compensation

**LaMeDuSe SAS**

*Annexe aux Conditions Générales de Vente : Services d'Hébergement*

*Dernière mise à jour : 16 juillet 2026*

---

## Préambule

La présente annexe (ci-après l'« **Annexe SLA** ») précise les engagements de niveau de service (*Service Level Agreement*) de **LaMeDuSe SAS** (ci-après « **LaMeDuSe** ») et le barème des compensations applicables en cas de non-respect de ces engagements. Elle constitue l'annexe SLA visée aux articles 12.1 et 12.3 des Conditions Générales de Vente Services d'Hébergement (ci-après les « **CGV** ») et à l'article 11.3 des Conditions Particulières Serveur dédié (ci-après les « **CP Serveur dédié** »).

Elle fait partie intégrante du contrat. En cas de contradiction, l'ordre de priorité prévu à l'article 37.3 des CGV s'applique : le Devis peut prévoir un engagement SLA différent (renforcé ou adapté) qui prévaut alors sur la présente Annexe.

L'avoir calculé selon la présente Annexe constitue la **seule et exclusive compensation** due par LaMeDuSe au titre d'un défaut de disponibilité, conformément à l'article 12.3 des CGV.

---

## Article 1 : Définitions

- **Taux de disponibilité** : pourcentage du temps, sur la période de mesure, pendant lequel le Service est disponible, calculé selon la formule de l'article 3.
- **Gamme de service** : niveau d'engagement de disponibilité applicable au Service, précisé au Devis parmi les trois niveaux définis à l'article 2 (Essentiel, Avancé ou Critique). À défaut d'indication au Devis, la gamme Essentiel s'applique.
- **Indisponibilité** : période continue d'au moins **cinq (5) minutes** durant laquelle le Service relevant de la responsabilité de LaMeDuSe est totalement inaccessible depuis l'extérieur, à l'exclusion des cas non comptabilisés prévus à l'article 4. Toute interruption d'une durée inférieure à cinq (5) minutes consécutives n'est pas comptabilisée comme Indisponibilité.
- **Période de mesure** : le mois civil, la disponibilité étant appréciée sur une base mensuelle glissante conformément à l'article 12.1 des CGV.
- **Panne matérielle** : tout incident résultant de la défaillance d'un composant matériel du serveur (disque, carte mère, mémoire, alimentation, ventilateur, carte réseau, etc.) entraînant l'indisponibilité complète du serveur concerné, à l'exclusion des problèmes de performance (latence, surchauffe, surcharge) qui ne constituent pas une indisponibilité.
- **Délai d'intervention** : temps écoulé entre le signalement d'un incident par le Client (ouverture d'un ticket recevable) et la prise en compte de cet incident par les équipes techniques de LaMeDuSe, à distinguer de la résolution effective de l'incident.
- **Avoir** : crédit accordé au Client, exprimé en pourcentage du montant mensuel hors taxes du Service concerné, imputable sur une facture ultérieure.
- **Montant mensuel de référence** : montant hors taxes facturé au titre du seul Service affecté par l'indisponibilité, pour le mois concerné.

---

## Article 2 : Engagement de disponibilité par gamme

2.1. LaMeDuSe garantit un taux de disponibilité mensuel pour l'infrastructure relevant de sa responsabilité (réseau, alimentation électrique, refroidissement, et pour les serveurs dédiés, l'infrastructure physique et réseau au sens de l'article 11 des CP Serveur dédié). Le niveau garanti dépend de la **gamme de service** souscrite, précisée au Devis, selon le barème suivant :

| Gamme de service | Taux de disponibilité mensuel garanti | Indisponibilité maximale tolérée (base 30 jours) |
|---|---|---|
| **Essentiel** | 99,9 % | environ 43 minutes et 50 secondes par mois |
| **Avancé** | 99,95 % | environ 21 minutes et 55 secondes par mois |
| **Critique** | 99,99 % | environ 4 minutes et 23 secondes par mois |

2.2. La gamme applicable à chaque Service est celle précisée au Devis. À défaut d'indication expresse au Devis, la gamme **Essentiel** (99,9 %) s'applique par défaut. Le Devis peut également prévoir un engagement de disponibilité renforcé ou adapté qui prévaut alors sur le présent barème, dans les conditions de l'article 37.3 des CGV.

2.3. Le SLA porte exclusivement sur les éléments relevant de la responsabilité de LaMeDuSe. Il ne couvre pas les indisponibilités imputables au système d'exploitation, aux applications, aux configurations ou aux manipulations du Client, conformément à l'article 11.2 des CP Serveur dédié.

---

## Article 3 : Méthode de calcul du taux de disponibilité

3.1. Le taux de disponibilité est calculé, pour chaque mois civil, selon la formule suivante :

```
Taux de disponibilité (%) = ((T − I) / T) × 100
```

où :
- **T** = durée totale du mois considéré, en minutes (hors périodes non comptabilisées au titre de l'article 4) ;
- **I** = durée cumulée des indisponibilités imputables à LaMeDuSe, en minutes, sur le mois considéré.

3.2. Les indisponibilités sont décomptées à partir de l'ouverture d'un ticket d'incident recevable par le Client ou, si elle est antérieure, à partir de leur constatation par les systèmes de supervision de LaMeDuSe, jusqu'au rétablissement effectif du Service. Seules sont comptabilisées les périodes d'indisponibilité continues d'au moins cinq (5) minutes, conformément à la définition de l'article 1.

3.3. En cas de litige sur la mesure, les journaux de supervision de LaMeDuSe font foi, sans préjudice du droit du Client de rapporter la preuve contraire, conformément à l'article 34 des CGV.

---

## Article 4 : Événements non comptabilisés

Conformément à l'article 12.2 des CGV, ne sont pas comptabilisés comme indisponibilité :

- les opérations de **maintenance planifiée**, notifiées au Client au moins **48 heures** à l'avance (art. 12.2 des CGV et 10.6 des CP Serveur dédié) ;
- les indisponibilités résultant d'un cas de **force majeure** au sens de l'article 27 des CGV ;
- les indisponibilités imputables au **Client**, à ses prestataires tiers, ou à des éléments hors du périmètre contractuel de LaMeDuSe (connexion internet du Client, applications tierces, système d'exploitation, configurations) ;
- les interruptions résultant d'une **attaque DoS/DDoS** ou des mesures de mitigation associées, dans les conditions des articles 15 des CGV et 9 des CP Serveur dédié ;
- les interruptions consécutives à une **suspension** régulière du Service (impayé, manquement à l'AUP, signalement d'abus non traité) prononcée conformément aux CGV et aux CP applicables.

---

## Article 5 : Barème de compensation (avoirs de disponibilité)

5.1. Lorsque le taux de disponibilité mensuel constaté est inférieur à l'engagement garanti pour la gamme souscrite (article 2), le Client peut, sur demande formulée dans les conditions de l'article 6, bénéficier d'un avoir calculé selon le barème suivant. Le seuil haut de déclenchement dépend de la gamme applicable au Service :

| Taux de disponibilité mensuel constaté (MAR) | | | Avoir (en % du montant mensuel HT du Service concerné) |
|---|---|---|---|
| **Gamme Essentiel (99,9 %)** | **Gamme Avancé (99,95 %)** | **Gamme Critique (99,99 %)** | |
| 99,0 % ≤ MAR < 99,9 % | 99,0 % ≤ MAR < 99,95 % | 99,0 % ≤ MAR < 99,99 % | 10 % |
| 95,0 % ≤ MAR < 99,0 % | 95,0 % ≤ MAR < 99,0 % | 95,0 % ≤ MAR < 99,0 % | 25 % |
| MAR < 95,0 % | MAR < 95,0 % | MAR < 95,0 % | 50 % |

5.2. L'avoir est calculé sur le **montant mensuel de référence** du seul Service affecté, à l'exclusion des autres Services, des options non affectées et des frais de mise en service (setup).

5.3. Le montant cumulé de l'ensemble des avoirs accordés au titre d'un même mois et d'un même Service, toutes causes confondues (avoir de disponibilité du présent article et avoir d'intervention de l'article 7), ne peut en aucun cas excéder **50 % du montant mensuel de référence** du Service concerné.

5.4. L'avoir prend la forme d'un crédit imputable sur une facture ultérieure. Il ne donne lieu à aucun remboursement en numéraire, sauf en cas de résiliation du Service ne permettant plus l'imputation de l'avoir, auquel cas son montant résiduel est remboursé.

---

## Article 6 : Modalités de demande et d'octroi

6.1. La demande d'avoir doit être formulée par le Client par écrit (ticket depuis l'espace client ou email à **support@lameduse.cloud**) dans un délai de **trente (30) jours** à compter de la fin du mois au titre duquel l'indisponibilité est constatée. À défaut, la demande est réputée abandonnée pour le mois concerné.

6.2. La demande précise les dates, heures et durées des indisponibilités constatées, ainsi que, le cas échéant, les références des tickets d'incident ouverts.

6.3. LaMeDuSe instruit la demande, la rapproche de ses journaux de supervision, et notifie sa décision au Client dans un délai raisonnable. L'avoir validé est imputé sur la facture du mois suivant son acceptation.

6.4. Le bénéfice de l'avoir est subordonné au fait que le Client soit à jour de ses paiements au titre du Service concerné.

---

## Article 7 : Dispositions spécifiques au Serveur dédié

7.1. Pour les Services de serveur dédié, outre l'engagement de disponibilité de l'article 2, LaMeDuSe s'engage à intervenir pour le diagnostic et le **remplacement d'un composant matériel défaillant sous deux (2) heures** à compter du signalement, sous réserve de la disponibilité de la pièce en stock local, conformément à l'article 10.3 des CP Serveur dédié.

7.2. Si la pièce n'est pas disponible en stock local, LaMeDuSe propose, dans le même délai de deux (2) heures, la bascule vers une **Unité de remplacement (swap)** de configuration identique ou équivalente, conformément à l'article 10.4 des CP Serveur dédié.

7.3. En cas de non-respect du délai d'intervention de deux (2) heures prévu à l'article 7.1 ou 7.2, imputable à LaMeDuSe, le Client peut bénéficier d'un avoir complémentaire de **5 % du montant mensuel HT** du serveur concerné par tranche entamée de **trente (30) minutes** de retard au-delà du délai garanti, dans la limite de **50 % du montant mensuel HT** du serveur concerné.

7.4. Les avoirs prévus au présent article se cumulent avec l'avoir de disponibilité de l'article 5, sans que le total des avoirs accordés au titre d'un même mois et d'un même serveur, toutes causes confondues, ne puisse excéder **50 % du montant mensuel de référence** de ce serveur, conformément à l'article 5.3.

---

## Article 8 : Support technique

8.1. Les niveaux de support (support standard aux horaires ouvrés, ou niveaux étendus tels que astreinte ou support 24/7) sont précisés au Devis, conformément à l'article 13 des CGV.

8.2. Lorsque des délais de prise en charge ou de résolution sont contractualisés au Devis, ils sont réputés compléter la présente Annexe SLA et prévalent, pour les éléments qu'ils couvrent, dans les conditions de l'article 37.3 des CGV.

---

## Article 9 : Limites

9.1. Les avoirs prévus par la présente Annexe constituent la seule et exclusive compensation due par LaMeDuSe au titre d'un défaut de disponibilité ou d'un dépassement des délais d'intervention, à l'exclusion de tout autre dédommagement, conformément aux articles 12.3 des CGV et 26 des CGV relatif à la responsabilité.

9.2. La présente Annexe s'inscrit dans le cadre de l'obligation de moyens de LaMeDuSe définie à l'article 16 des CGV, sous réserve des engagements chiffrés de résultat qu'elle prévoit expressément (taux de disponibilité et, pour le serveur dédié, délai de remplacement matériel).

---

*Document établi par LaMeDuSe SAS · SIREN 915 248 579 · 231 rue Saint-Honoré, 75001 Paris.*

*Dernière mise à jour : 16 juillet 2026*