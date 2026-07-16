# Conditions Particulières : Service de Serveur Virtuel (VPS)

**LaMeDuSe SAS**

---

## Préambule

Les présentes Conditions Particulières (ci-après les « **CP** ») complètent et précisent les Conditions Générales de Vente Services d'Hébergement de LaMeDuSe SAS (ci-après les « **CGV** ») pour ce qui concerne spécifiquement le service de **serveur virtuel** ou **VPS** (*Virtual Private Server*, ci-après le « **Service** »).

Conformément à l'article 37.3 des CGV, en cas de contradiction entre les documents contractuels, l'ordre de priorité suivant s'applique : (i) le Devis ou Bon de Commande, (ii) les présentes CP, (iii) les CGV, (iv) les autres annexes. Pour tout point non traité par les présentes CP, les dispositions des CGV s'appliquent pleinement.

---

## Article 1 : Objet

Les présentes CP ont pour objet de définir les conditions techniques, financières et contractuelles spécifiques applicables à la fourniture par LaMeDuSe d'un ou plusieurs serveurs virtuels, correspondant à des ressources de calcul, de mémoire et de stockage virtualisées et allouées au Client sur une infrastructure mutualisée, dans les conditions décrites au Devis.

---

## Article 2 : Définitions spécifiques

- **VPS (serveur virtuel)** : instance virtualisée disposant de ressources dédiées (vCPU, mémoire vive, stockage) allouées au Client sur un hôte physique mutualisé exploité par LaMeDuSe.
- **Hyperviseur** : couche logicielle de virtualisation, exploitée et maintenue par LaMeDuSe, permettant l'exécution de plusieurs VPS sur un même hôte physique.
- **Hôte physique** : serveur physique de LaMeDuSe hébergeant un ou plusieurs VPS.
- **Snapshot** : copie ponctuelle de l'état d'un VPS à un instant donné, lorsque cette fonctionnalité est incluse ou souscrite au Devis.
- **Interface de gestion** : espace client ou console permettant au Client de démarrer, arrêter, réinstaller ou reconfigurer son VPS de manière autonome.

---

## Article 3 : Description du Service et localisation

3.1. Le VPS est livré avec la configuration (vCPU, mémoire, capacité et type de stockage, bande passante) précisée au Devis. Toute modification de configuration s'effectue selon les options disponibles, le cas échéant par simple montée en gamme depuis l'interface de gestion ou par avenant.

3.2. Sauf mention contraire au Devis, le VPS est livré avec un système d'exploitation de base sélectionné par le Client parmi les images proposées par LaMeDuSe. L'administration, la sécurisation et la mise à jour du système d'exploitation et des applicatifs relèvent ensuite de la seule responsabilité du Client, conformément à l'article 11 des présentes CP.

3.3. Le Client dispose d'un accès autonome à son VPS (interface de gestion, accès console, accès distant de type SSH ou équivalent), lui permettant de le gérer, y compris en cas de dysfonctionnement de son système d'exploitation.

3.4. Le VPS est hébergé dans un Datacenter situé en **France, en Allemagne ou en Suisse**, le pays précis étant indiqué au Devis, conformément à l'article 4 des CGV.

---

## Article 4 : Commande et mise à disposition

4.1. Toute commande de VPS fait l'objet d'un Devis précisant la configuration, le Datacenter de rattachement, la durée d'engagement éventuelle et le tarif applicable.

4.2. Le VPS étant provisionné de manière automatisée, sa mise à disposition intervient en principe dans un délai court à compter de la validation du Devis et de la réception du premier paiement. LaMeDuSe communique les accès au Client par un canal sécurisé.

---

## Article 5 : Durée, engagement et renouvellement

5.1. Sauf stipulation contraire au Devis, le Service est souscrit sans engagement de durée minimale, avec facturation mensuelle et résiliation possible à tout moment moyennant le préavis prévu à l'article 12 des présentes CP.

5.2. Le Client peut opter pour une durée d'engagement (12 ou 24 mois) en contrepartie d'une remise tarifaire précisée au Devis, dans les conditions de l'article 8 des CGV.

5.3. À l'échéance d'une éventuelle période d'engagement, le Service est reconduit tacitement dans les conditions de l'article 8.2 des CGV, sauf notification de non-reconduction adressée au moins **trente (30) jours calendaires** avant le terme de la période en cours.

---

## Article 6 : Ressources partagées et usage raisonnable

6.1. Le VPS repose sur une infrastructure mutualisée. Les ressources garanties (vCPU, mémoire, stockage) sont celles précisées au Devis. Le Client s'engage à respecter les quotas raisonnables d'utilisation permettant de garantir la qualité de service pour l'ensemble des utilisateurs de l'hôte, conformément à l'article 3 de l'AUP.

6.2. Un usage anormalement élevé ou portant atteinte à la stabilité de l'hôte physique ou des autres VPS peut donner lieu à une alerte, une limitation technique, ou une proposition de montée en gamme, dans les conditions des articles 14.3 des CGV et 3 de l'AUP.

---

## Article 7 : Bande passante et trafic réseau

7.1. Le VPS est raccordé selon le débit et le volume de trafic mensuel inclus précisés au Devis (offre mesurée ou non mesurée selon le cas).

7.2. En cas d'offre à trafic mesuré, tout dépassement du volume inclus est facturé selon le tarif indiqué au Devis, ou entraîne une limitation de débit (throttling) au choix précisé au Devis.

7.3. Le Client s'engage à ne pas utiliser le VPS pour émettre un trafic anormal, abusif ou portant atteinte à l'intégrité du réseau de LaMeDuSe ou de ses fournisseurs, conformément à l'article 2 de l'AUP.

---

## Article 8 : Protection anti-DDoS

8.1. Sauf mention contraire au Devis, le VPS bénéficie de la protection anti-DDoS de base incluse au niveau du réseau de LaMeDuSe, opérant aux couches réseau et transport (L3/L4), dans les conditions de l'article 15 des CGV.

8.2. Les interruptions liées à une attaque DDoS ou aux mesures de mitigation associées ne sont pas comptabilisées dans le calcul du SLA, conformément aux articles 12.2 et 15.3 des CGV.

---

## Article 9 : Sauvegarde et snapshots

9.1. Sauf option de sauvegarde ou de snapshots managés souscrite au Devis, LaMeDuSe n'assure aucune sauvegarde des données présentes sur le VPS. Il appartient au Client de mettre en œuvre sa propre politique de sauvegarde.

9.2. Lorsqu'une option de sauvegarde ou de snapshots est souscrite, ses modalités (fréquence, durée de rétention, procédure de restauration) sont précisées au Devis.

9.3. En cas d'incident affectant l'hôte physique, les données du VPS qui n'auraient pas fait l'objet d'une sauvegarde par le Client peuvent être définitivement perdues, sous réserve des mesures de redondance éventuellement incluses et précisées au Devis.

---

## Article 10 : Niveau de service (SLA)

10.1. LaMeDuSe garantit, pour l'infrastructure de virtualisation relevant de sa responsabilité (hôtes physiques, hyperviseur, réseau, alimentation et refroidissement du Datacenter), un taux de disponibilité mensuel qui dépend de la **gamme de service** souscrite et précisée au Devis (**99,9 %** pour la gamme Essentiel, **99,95 %** pour la gamme Avancé, **99,99 %** pour la gamme Critique), mesuré sur une base mensuelle glissante, dans les conditions et exclusions prévues à l'article 12 des CGV et à l'annexe SLA. À défaut d'indication de gamme au Devis, la gamme Essentiel (99,9 %) s'applique.

10.2. Ce SLA porte exclusivement sur la disponibilité de l'infrastructure mise à disposition par LaMeDuSe. Il ne couvre pas les indisponibilités résultant du système d'exploitation, des applications, des configurations ou des manipulations effectuées par le Client sur le VPS, celles-ci relevant de sa seule responsabilité.

---

## Article 11 : Responsabilités du Client

11.1. Le Client est seul responsable :
   - de l'administration, de la configuration et de la sécurisation du système d'exploitation et des applications installées sur le VPS ;
   - de la mise à jour régulière des correctifs de sécurité ;
   - de la sauvegarde de ses données, sauf option souscrite au Devis ;
   - de l'usage conforme du VPS au regard de la réglementation applicable et de l'AUP prévue à l'article 14 des CGV.

11.2. Le Client garantit LaMeDuSe contre toute conséquence dommageable résultant d'un défaut de sécurisation du VPS dont il a la charge, notamment en cas de compromission utilisée pour porter atteinte à des tiers.

---

## Article 12 : Suspension et résiliation

12.1. En cas de manquement du Client à ses obligations (impayé, usage abusif, atteinte à la sécurité du réseau, signalement d'abus non traité), LaMeDuSe applique les modalités de suspension prévues aux articles 10.5, 14.4 et 18 des CGV et à l'AUP.

12.2. Hors engagement de durée, la résiliation du Service par le Client s'effectue avec un préavis de **trente (30) jours calendaires** avant la fin de la période de facturation en cours. S'agissant d'un Service engagé, la résiliation anticipée s'effectue dans les conditions de l'article 8.4 des CGV.

---

## Article 13 : Sort des données en fin de contrat

13.1. Il appartient au Client d'avoir réalisé, avant la date d'effet de la résiliation ou de l'expiration du Service, l'ensemble des sauvegardes et exports de ses données. À la date d'effet de la résiliation, l'accès au VPS est coupé.

13.2. La restitution et la suppression des Données s'effectuent dans les conditions de réversibilité de l'article 9 des CGV, la période de conservation de **trente (30) jours** prévue à l'article 9.2 des CGV s'appliquant, sauf disposition contraire au Devis.

---

## Article 14 : Obligation légale d'identification (LCEN)

Conformément au V de l'article 6 de la loi n° 2004-575 du 21 juin 2004 pour la confiance dans l'économie numérique (LCEN), dans sa rédaction issue de la loi n° 2024-449 du 21 mai 2024, et à l'article L. 34-1 du Code des postes et des communications électroniques, LaMeDuSe, en sa qualité de fournisseur de services d'hébergement, détient et conserve les données de nature à permettre l'identification des contributeurs aux contenus, dans les conditions de l'article 19 des CGV. Le Client s'engage à fournir des informations d'identification exactes et à jour, conformément à l'article 6 des CGV.

---

## Article 15 : Articulation avec les CGV

Pour tout point non expressément traité par les présentes CP (facturation, responsabilité, données personnelles, force majeure, résiliation pour manquement, droit applicable, juridiction compétente), les dispositions des CGV Hébergement LaMeDuSe s'appliquent pleinement et sans réserve.

---

*Dernière mise à jour : 16 juillet 2026*
