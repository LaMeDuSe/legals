# Conditions Particulières : Service de Serveur Dédié

**LaMeDuSe SAS**

---

## Préambule

Les présentes Conditions Particulières (ci-après les « **CP** ») complètent et précisent les Conditions Générales de Vente Services d'Hébergement de LaMeDuSe SAS (ci-après les « **CGV** ») pour ce qui concerne spécifiquement le service de **serveur dédié** (ci-après le « **Service** »).

Conformément à l'article 37.3 des CGV, en cas de contradiction entre les documents contractuels, l'ordre de priorité suivant s'applique : (i) le Devis ou Bon de Commande, (ii) les présentes CP, (iii) les CGV, (iv) les autres annexes. Pour tout point non traité par les présentes CP, les dispositions des CGV s'appliquent pleinement.

---

## Article 1 : Objet

Les présentes CP ont pour objet de définir les conditions techniques, financières et contractuelles spécifiques applicables à la fourniture par LaMeDuSe d'un ou plusieurs serveurs physiques dédiés, non mutualisés avec d'autres clients, mis à disposition du Client dans les conditions décrites au Devis.

---

## Article 2 : Définitions spécifiques

- **Serveur dédié** : machine physique entière (CPU, RAM, stockage, carte réseau) allouée exclusivement au Client, à l'exclusion de tout partage de ressources matérielles avec un autre client de LaMeDuSe.
- **Datacenter** : site d'hébergement physique dans lequel le Serveur est installé, exploité par LaMeDuSe ou par un sous-traitant hébergeur désigné.
- **Accès KVM/IPMI** : accès distant hors bande permettant au Client de contrôler le Serveur (écran, clavier, redémarrage, réinstallation) indépendamment de l'état de son système d'exploitation.
- **Remote Hands** : intervention physique manuelle réalisée par le personnel du Datacenter sur demande du Client ou de LaMeDuSe (redémarrage physique, remplacement de composant, branchement).
- **Fenêtre de maintenance** : plage horaire notifiée au Client pendant laquelle une intervention planifiée sur l'infrastructure réseau ou électrique du Datacenter peut entraîner une interruption du Service.
- **Unité de remplacement (swap)** : serveur physique de secours, de configuration identique ou équivalente, mis à disposition du Client en remplacement du Serveur initial lorsque le composant défaillant n'est pas disponible en stock local.

---

## Article 3 : Description du Service et localisation

3.1. Le Serveur est livré avec la configuration matérielle (processeur, mémoire vive, capacité et type de stockage, carte(s) réseau) précisée au Devis. Toute modification de configuration fait l'objet d'un avenant ou d'un nouveau Devis.

3.2. Sauf mention contraire au Devis, le Serveur est livré nu ou avec un système d'exploitation de base installé par LaMeDuSe à la demande du Client ; l'administration, la sécurisation et la mise à jour du système d'exploitation et des applicatifs relèvent ensuite de la seule responsabilité du Client, conformément à l'article 12 des présentes CP.

3.3. Le Client dispose d'un accès KVM/IPMI lui permettant de gérer le Serveur de manière autonome, y compris en cas de dysfonctionnement du système d'exploitation.

3.4. Le Serveur est hébergé dans un Datacenter situé en **France, en Allemagne ou en Suisse**, le pays précis étant indiqué au Devis. Toute relocalisation du Serveur vers un autre Datacenter, y compris au sein d'un même pays, est notifiée au Client par écrit avec un préavis minimal de **cinq (5) jours calendaires**, sauf urgence de sécurité ou cas de force majeure imposant un délai plus court.

---

## Article 4 : Commande et mise à disposition

4.1. Toute commande de Serveur dédié fait l'objet d'un Devis précisant la configuration, le Datacenter de rattachement, la durée d'engagement éventuelle et le tarif applicable.

4.2. Le délai de mise à disposition standard est de **24 à 72 heures ouvrées** à compter de la validation du Devis et de la réception du premier paiement, pour une configuration standard disponible en stock. Pour toute configuration sur mesure nécessitant une commande de matériel spécifique, le délai est communiqué au Client lors de l'établissement du Devis et peut être porté jusqu'à **quinze (15) jours ouvrés**.

4.3. LaMeDuSe informe le Client par écrit de la mise à disposition effective du Serveur et lui transmet les identifiants d'accès (accès KVM/IPMI, identifiants système le cas échéant) par un canal sécurisé.

---

## Article 5 : Durée, engagement et renouvellement

5.1. Sauf stipulation contraire au Devis, le Service est souscrit sans engagement de durée minimale, avec facturation mensuelle et résiliation possible à tout moment moyennant le préavis prévu à l'article 15 des présentes CP.

5.2. Le Client peut opter pour une durée d'engagement (12 ou 24 mois) en contrepartie d'une remise tarifaire précisée au Devis. **Le tarif applicable pendant toute la durée de l'engagement souscrit est fixe** : il ne peut faire l'objet d'aucune révision, y compris au titre de l'article 10.6 des CGV, avant le terme de la période d'engagement en cours. Toute révision tarifaire décidée par LaMeDuSe ne s'applique qu'à compter du renouvellement du Service.

5.3. À l'échéance de la période d'engagement, le Service est **reconduit tacitement pour une durée identique** à celle initialement souscrite, sauf notification de non-reconduction adressée par l'une des Parties à l'autre au moins **trente (30) jours calendaires** avant le terme de la période en cours. Le tarif applicable à la période reconduite est celui en vigueur à la date de renouvellement, communiqué au Client préalablement dans les conditions de l'article 10.6 des CGV.

5.4. Toute résiliation anticipée d'un Service engagé donne lieu à l'application des conditions de résiliation anticipée prévues à l'article 15.2 des présentes CP.

---

## Article 6 : Accès et sécurité

6.1. Les identifiants d'accès (KVM/IPMI, comptes d'administration) sont strictement personnels et confidentiels. Le Client est seul responsable de leur conservation et de toute utilisation qui en serait faite, y compris par un tiers non autorisé.

6.2. LaMeDuSe met en œuvre les mesures de sécurité physique du Datacenter (contrôle d'accès, vidéosurveillance) mais n'a pas accès, sauf demande expresse du Client dans le cadre d'une intervention Remote Hands ou d'une obligation légale, au contenu du Serveur ni aux données qui y sont hébergées.

6.3. Toute intervention de LaMeDuSe sur le Serveur nécessitant un accès aux données du Client (support technique, diagnostic) requiert l'autorisation préalable du Client, sauf urgence de sécurité mettant en cause l'infrastructure mutualisée de LaMeDuSe ou de tiers.

---

## Article 7 : Bande passante et trafic réseau

7.1. Le Serveur est raccordé selon le débit et le volume de trafic mensuel inclus précisés au Devis (offre mesurée ou non mesurée selon le cas).

7.2. En cas d'offre à trafic mesuré, tout dépassement du volume inclus est facturé selon le tarif au Go indiqué au Devis, ou entraîne une limitation de débit (throttling) au choix précisé au Devis.

7.3. Le Client s'engage à ne pas utiliser le Serveur pour émettre un trafic anormal, abusif ou portant atteinte à l'intégrité du réseau de LaMeDuSe ou de ses fournisseurs (spam, scan de ports à grande échelle, déni de service émis).

---

## Article 8 : Adresses IP

8.1. Le Serveur est livré avec le nombre d'adresses IP précisé au Devis. Toute adresse IP supplémentaire est soumise à la justification d'usage exigée par les politiques d'allocation en vigueur (notamment les règles du RIPE NCC), le Client s'engageant à fournir à première demande toute information nécessaire à cette justification.

8.2. Les adresses IP allouées au Client dans le cadre du Service demeurent la propriété de LaMeDuSe ou du registre régional concerné et lui sont attribuées à titre d'usage pour la durée du Service. **Elles ne sont en aucun cas portables** : à la résiliation ou à l'expiration du Service, quelle qu'en soit la cause, les adresses IP sont restituées et réaffectées par LaMeDuSe, sans possibilité de transfert vers un autre hébergeur ou une autre infrastructure.

---

## Article 9 : Protection anti-DDoS

9.1. Sauf mention contraire au Devis, le Serveur bénéficie d'une protection anti-DDoS de base incluse, opérant aux **couches réseau et transport (L3/L4)**, assurant un filtrage automatique du trafic volumétrique manifestement malveillant au niveau du réseau de LaMeDuSe.

9.2. Une protection complémentaire au niveau applicatif (**couche 7 / L7**), couvrant notamment les attaques HTTP/HTTPS applicatives, peut être souscrite en option et est alors précisée au Devis.

9.3. En cas d'attaque dépassant les capacités de la protection souscrite, LaMeDuSe peut, à titre conservatoire et sans préavis, appliquer une mesure de mitigation (null-route temporaire de l'IP visée, filtrage renforcé) afin de préserver l'intégrité de son réseau. Le Client en est informé dans les meilleurs délais et la mesure est levée dès que la menace est écartée.

9.4. Les interruptions liées à une attaque DDoS ou aux mesures de mitigation associées ne sont pas comptabilisées dans le calcul du SLA, conformément aux articles 12.2 et 15.3 des CGV.

---

## Article 10 : Maintenance et remplacement matériel

10.1. LaMeDuSe assure la maintenance de l'infrastructure physique du Serveur (alimentation électrique, connectivité réseau, climatisation du Datacenter) et le remplacement de tout composant matériel défaillant relevant de sa responsabilité (disque, mémoire, alimentation, carte réseau).

10.2. Le Client configure librement la structure de stockage de son Serveur (RAID logiciel ou matériel, niveau de RAID, répartition des volumes), selon les options disponibles pour la configuration souscrite au Devis.

10.3. En cas de panne matérielle avérée et non imputable au Client, LaMeDuSe s'engage à intervenir pour diagnostic et **remplacement du composant défaillant sous deux (2) heures** à compter du signalement, sous réserve de la disponibilité de la pièce en stock local. LaMeDuSe maintient à cet effet un stock de pièces et disques de secours dans chaque Datacenter d'exploitation.

10.4. Si le composant nécessaire n'est pas disponible en stock local au moment du signalement, LaMeDuSe en informe immédiatement le Client et propose, dans le même délai de deux (2) heures, la bascule du Client vers une **Unité de remplacement (swap)** de configuration identique ou équivalente, le temps que la pièce d'origine soit approvisionnée ou que le Serveur initial soit remis en service.

10.5. Les données stockées sur le Serveur ne sont pas sauvegardées par LaMeDuSe sauf option de sauvegarde managée souscrite séparément au Devis. En cas de remplacement d'un disque défaillant ou de bascule vers une Unité de remplacement, les données qui n'auraient pas fait l'objet d'une sauvegarde par le Client peuvent être définitivement perdues ; il appartient au Client de mettre en œuvre sa propre politique de sauvegarde conformément à l'article 12 des présentes CP.

10.6. Toute intervention de maintenance planifiée sur l'infrastructure du Datacenter (réseau, électrique) est notifiée au Client au moins 48 heures à l'avance, sauf urgence de sécurité.

---

## Article 11 : Niveau de service (SLA) spécifique au Serveur dédié

11.1. LaMeDuSe garantit, pour l'infrastructure relevant de sa responsabilité (réseau, alimentation électrique, climatisation du Datacenter), un taux de disponibilité mensuel de **99,9 %**, mesuré sur une base mensuelle glissante, dans les conditions et exclusions prévues à l'article 12 des CGV et à l'annexe SLA.

11.2. Ce SLA porte exclusivement sur la disponibilité de l'infrastructure physique et réseau mise à disposition par LaMeDuSe. Il ne couvre pas les indisponibilités résultant du système d'exploitation, des applications, des configurations ou des manipulations effectuées par le Client sur le Serveur, celles-ci relevant de sa seule responsabilité.

11.3. En cas de panne matérielle imputable à LaMeDuSe et non traitée dans le délai prévu à l'article 10.3 ou 10.4, le Client peut bénéficier d'un avoir calculé selon le barème SLA applicable, dans les conditions de l'article 12.3 des CGV.

---

## Article 12 : Responsabilités du Client

12.1. Le Client est seul responsable :
   - de l'administration, de la configuration et de la sécurisation du système d'exploitation et des applications installées sur le Serveur ;
   - de la mise à jour régulière des correctifs de sécurité ;
   - de la sauvegarde de ses données, sauf option de sauvegarde managée souscrite au Devis ;
   - de l'usage conforme du Serveur au regard de la réglementation applicable et de la Politique d'Usage Acceptable (AUP) prévue à l'article 14 des CGV.

12.2. Le Client garantit LaMeDuSe contre toute conséquence dommageable résultant d'un défaut de sécurisation du Serveur dont il a la charge, notamment en cas de compromission du système utilisée pour porter atteinte à des tiers.

---

## Article 13 : Obligation légale d'identification (LCEN)

13.1. Conformément aux articles 6-II et 6-VI de la loi n° 2004-575 du 21 juin 2004 pour la confiance dans l'économie numérique (LCEN), LaMeDuSe, en sa qualité d'hébergeur, conserve pendant une durée d'un (1) an les données de nature à permettre l'identification de toute personne ayant contribué à la création d'un contenu hébergé sur le Serveur, et peut être tenue de les communiquer à l'autorité judiciaire sur réquisition.

13.2. Le Client s'engage à fournir à LaMeDuSe des informations d'identification exactes et à jour lors de la souscription du Service, et à les maintenir à jour pendant toute la durée du contrat.

---

## Article 14 : Politique d'abus (Abuse)

14.1. Tout signalement d'abus concernant un usage du Serveur (spam, phishing, contenu illicite, activité malveillante) peut être adressé par un tiers ou une autorité à l'adresse **abuse@lameduse.cloud**.

14.2. Dès réception d'un signalement recevable, LaMeDuSe le transmet au Client, qui dispose d'un délai de **vingt-quatre (24) heures** pour y répondre et, le cas échéant, remédier au manquement signalé.

14.3. À défaut de réponse ou de mesure corrective dans ce délai, ou en cas de signalement présentant un caractère d'urgence ou de gravité manifeste (contenu manifestement illicite, atteinte active à des tiers), LaMeDuSe peut suspendre le Service concerné sans préavis, à titre conservatoire, dans les conditions de l'article 15.1 des présentes CP, sans préjudice de son droit à résiliation.

---

## Article 15 : Suspension et résiliation

15.1. En cas de manquement du Client à ses obligations (impayé, usage abusif, atteinte à la sécurité du réseau, signalement d'abus non traité), LaMeDuSe applique les modalités de suspension prévues aux articles 10.5, 14.4 et 18 des CGV et à l'article 14 des présentes CP.

15.2. En cas de résiliation anticipée par le Client d'un Service souscrit avec engagement de durée (article 5.2 des présentes CP), les mensualités restant dues jusqu'au terme de la période d'engagement initialement souscrite restent exigibles, sauf accord contraire de LaMeDuSe.

15.3. Hors engagement de durée, la résiliation du Service par le Client s'effectue avec un préavis de **trente (30) jours calendaires** avant la fin de la période de facturation en cours. S'agissant d'un Service engagé, la non-reconduction s'effectue conformément à l'article 5.3 des présentes CP.

---

## Article 16 : Sort du matériel et des données en fin de contrat

16.1. Il appartient au Client d'avoir réalisé, avant la date d'effet de la résiliation ou de l'expiration du Service, l'ensemble des sauvegardes et exports de ses données, conformément à sa responsabilité de sauvegarde prévue aux articles 10.5 et 12 des présentes CP. À la date d'effet de la résiliation, l'accès au Serveur est coupé.

16.2. Le Client dispose, à compter de la date d'effet de la résiliation, d'un délai de **sept (7) jours calendaires** pendant lequel il peut solliciter de LaMeDuSe la restitution d'une sauvegarde des données présentes sur le Serveur, sous réserve que celles-ci n'aient pas encore été effacées et que le Client soit à jour de ses paiements. Cette prestation de restitution assistée fait l'objet d'une facturation, dont le tarif est communiqué au Client préalablement à son exécution et soumis à son accord exprès.

16.3. Passé ce délai de sept (7) jours, LaMeDuSe procède à l'effacement sécurisé des données présentes sur le Serveur et à sa remise en disponibilité pour un autre client. Toute demande de restitution formée après ce délai ne pourra être satisfaite que dans l'hypothèse où le Serveur n'aurait pas encore été effacé ni réaffecté, sans que LaMeDuSe n'y soit tenue et sans qu'aucune réclamation ne puisse être formée à ce titre.

16.4. Le matériel constituant le Serveur reste en toute circonstance la propriété de LaMeDuSe (ou de son fournisseur Datacenter), sauf mention contraire expresse au Devis prévoyant une vente du matériel. Les adresses IP allouées suivent le régime de non-portabilité prévu à l'article 8.2 des présentes CP.

---

## Article 17 : Tarification

17.1. Le tarif du Service comprend, sauf mention contraire au Devis, la mise à disposition du matériel, la connectivité réseau incluse, l'accès KVM/IPMI et la maintenance de l'infrastructure physique.

17.2. Des frais de mise en service (setup) peuvent être appliqués lors de la première commande ou lors d'un changement de configuration matérielle, selon le barème en vigueur au Devis.

17.3. Toute option complémentaire (sauvegarde managée, bande passante additionnelle, adresses IP supplémentaires, protection anti-DDoS L7) est facturée selon les tarifs indiqués au Devis ou communiqués par LaMeDuSe.

---

## Article 18 : Droit de rétractation

18.1. Lorsque le Client a la qualité de consommateur au sens du Code de la consommation, il bénéficie en principe d'un délai de rétractation de quatorze (14) jours prévu à l'article L221-18 du Code de la consommation.

18.2. Ce droit ne peut toutefois être exercé, conformément à l'article L221-28 1° du Code de la consommation, dès lors que l'exécution du Service a commencé, avec l'accord préalable et exprès du Client et renoncement exprès de sa part à son droit de rétractation, avant la fin du délai de rétractation. La mise à disposition effective du Serveur au sens de l'article 4.3 des présentes CP, demandée et acceptée par le Client, vaut demande expresse d'exécution immédiate emportant renonciation au droit de rétractation dès cette mise à disposition.

---

## Article 19 : Articulation avec les CGV

Pour tout point non expressément traité par les présentes CP (facturation, responsabilité, données personnelles, force majeure, résiliation pour manquement, droit applicable, juridiction compétente), les dispositions des CGV Hébergement LaMeDuSe s'appliquent pleinement et sans réserve.

*Dernière mise à jour : 19 juin 2026*