# Annexe SLA : Niveaux de Service et Barème de Compensation

**LaMeDuSe SAS**

*Annexe aux Conditions Générales de Vente : Services d'Hébergement*

*Dernière mise à jour : 19 juin 2026*

---

## Préambule

La présente annexe (ci-après l'« **Annexe SLA** ») précise les engagements de niveau de service (*Service Level Agreement*) de **LaMeDuSe SAS** (ci-après « **LaMeDuSe** ») et le barème des compensations applicables en cas de non-respect de ces engagements. Elle constitue l'annexe SLA visée aux articles 12.1 et 12.3 des Conditions Générales de Vente Services d'Hébergement (ci-après les « **CGV** ») et à l'article 11.3 des Conditions Particulières Serveur dédié (ci-après les « **CP Serveur dédié** »).

Elle fait partie intégrante du contrat. En cas de contradiction, l'ordre de priorité prévu à l'article 37.3 des CGV s'applique : le Devis peut prévoir un engagement SLA différent (renforcé ou adapté) qui prévaut alors sur la présente Annexe.

L'avoir calculé selon la présente Annexe constitue la **seule et exclusive compensation** due par LaMeDuSe au titre d'un défaut de disponibilité, conformément à l'article 12.3 des CGV.

---

## Article 1 : Définitions

- **Taux de disponibilité** : pourcentage du temps, sur la période de mesure, pendant lequel le Service est disponible, calculé selon la formule de l'article 3.
- **Indisponibilité** : période durant laquelle le Service relevant de la responsabilité de LaMeDuSe est totalement inaccessible, à l'exclusion des cas non comptabilisés prévus à l'article 4.
- **Période de mesure** : le mois civil, la disponibilité étant appréciée sur une base mensuelle glissante conformément à l'article 12.1 des CGV.
- **Avoir** : crédit accordé au Client, exprimé en pourcentage du montant mensuel hors taxes du Service concerné, imputable sur une facture ultérieure.
- **Montant mensuel de référence** : montant hors taxes facturé au titre du seul Service affecté par l'indisponibilité, pour le mois concerné.

---

## Article 2 : Engagement de disponibilité

2.1. Sauf engagement différent précisé au Devis, LaMeDuSe garantit un taux de disponibilité mensuel de **99,9 %** pour l'infrastructure relevant de sa responsabilité (réseau, alimentation électrique, refroidissement, et pour les serveurs dédiés, l'infrastructure physique et réseau au sens de l'article 11 des CP Serveur dédié).

2.2. Un taux de disponibilité de 99,9 % correspond à une indisponibilité maximale tolérée d'environ **43 minutes et 50 secondes par mois** (base de 30 jours).

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

3.2. Les indisponibilités sont décomptées à partir de leur constatation par les systèmes de supervision de LaMeDuSe ou, si elle est antérieure, à partir de l'ouverture d'un ticket d'incident recevable par le Client, jusqu'au rétablissement effectif du Service.

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

## Article 5 : Barème de compensation (avoirs)

5.1. Lorsque le taux de disponibilité mensuel constaté est inférieur à l'engagement de 99,9 %, le Client peut, sur demande formulée dans les conditions de l'article 6, bénéficier d'un avoir calculé selon le barème suivant :

| Taux de disponibilité mensuel constaté | Avoir (en % du montant mensuel HT du Service concerné) |
|---|---|
| De 99,0 % à moins de 99,9 % | 5 % |
| De 98,0 % à moins de 99,0 % | 10 % |
| De 95,0 % à moins de 98,0 % | 25 % |
| De 90,0 % à moins de 95,0 % | 50 % |
| Inférieur à 90,0 % | 100 % |

5.2. L'avoir est calculé sur le **montant mensuel de référence** du seul Service affecté, à l'exclusion des autres Services, des options non affectées et des frais de mise en service (setup).

5.3. Le montant cumulé des avoirs accordés au titre d'un même mois ne peut en aucun cas excéder **100 % du montant mensuel de référence** du Service concerné.

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

7.3. En cas de non-respect du délai d'intervention de deux (2) heures prévu à l'article 7.1 ou 7.2, imputable à LaMeDuSe, le Client peut bénéficier d'un avoir complémentaire de **10 % du montant mensuel HT** du serveur concerné par tranche entamée de deux (2) heures de retard, dans la limite de **50 % du montant mensuel HT** du serveur concerné.

7.4. Les avoirs prévus au présent article se cumulent avec l'avoir de disponibilité de l'article 5, sans que le total des avoirs accordés au titre d'un même mois et d'un même serveur ne puisse excéder **100 % du montant mensuel de référence** de ce serveur.

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

*Dernière mise à jour : 19 juin 2026*
