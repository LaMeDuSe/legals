# Conditions Particulières : Service de Stockage Objet (S3)

**LaMeDuSe SAS**

---

## Préambule

Les présentes Conditions Particulières (ci-après les « **CP** ») complètent et précisent les Conditions Générales de Vente Services d'Hébergement de LaMeDuSe SAS (ci-après les « **CGV** ») pour ce qui concerne spécifiquement le service de **stockage objet** compatible avec le protocole S3 (ci-après le « **Service** »).

Conformément à l'article 37.3 des CGV, en cas de contradiction entre les documents contractuels, l'ordre de priorité suivant s'applique : (i) le Devis ou Bon de Commande, (ii) les présentes CP, (iii) les CGV, (iv) les autres annexes. Pour tout point non traité par les présentes CP, les dispositions des CGV s'appliquent pleinement.

---

## Article 1 : Objet

Les présentes CP ont pour objet de définir les conditions spécifiques applicables à la fourniture par LaMeDuSe d'un service de stockage objet, accessible via une interface programmatique compatible avec le protocole S3, permettant au Client de stocker et de récupérer des données sous forme d'objets organisés en conteneurs (buckets), dans les conditions décrites au Devis.

---

## Article 2 : Définitions spécifiques

- **Objet** : unité de donnée stockée (fichier et ses métadonnées associées) au sein du Service.
- **Bucket (conteneur)** : espace logique regroupant des objets, identifié par un nom unique et associé aux clés d'accès du Client.
- **Clés d'accès** : identifiants (clé d'accès et clé secrète) permettant au Client et à ses applications d'accéder au Service via l'API compatible S3.
- **Protocole S3** : interface de programmation compatible avec le standard de stockage objet du même nom, permettant l'interopérabilité avec les outils et bibliothèques usuels.
- **Trafic sortant (egress)** : volume de données extraites du Service vers l'extérieur, susceptible d'être facturé selon les modalités du Devis.

---

## Article 3 : Description du Service et localisation

3.1. Le Service met à disposition du Client une capacité de stockage objet facturée selon le volume stocké, le trafic et le nombre de requêtes, selon les modalités précisées au Devis.

3.2. Le Client accède au Service au moyen de ses clés d'accès, dont il est seul responsable de la conservation et de la confidentialité, conformément à l'article 6 des CGV.

3.3. Le Service assure la durabilité et la redondance des données au sein de la plateforme : chaque objet est répliqué sur plusieurs supports par LaMeDuSe, de manière à préserver l'intégrité des données stockées contre la défaillance d'un support matériel. Le niveau de résilience renforcé (par exemple réplication sur plusieurs sites ou zones) et les fonctionnalités de protection contre les erreurs du Client (versioning, verrouillage d'objet) sont précisés au Devis ou activés par le Client, dans les conditions de l'article 6 des présentes CP.

3.4. Les Données sont stockées dans un Datacenter situé en **France, en Allemagne ou en Suisse**, la localisation retenue étant indiquée au Devis, conformément à l'article 4 des CGV.

---

## Article 4 : Commande et mise à disposition

4.1. Toute commande fait l'objet d'un Devis précisant le modèle de facturation (volume, requêtes, trafic sortant), la localisation et les éventuelles options.

4.2. Le Service étant provisionné de manière automatisée, l'accès (clés, point d'accès de l'API) est communiqué au Client par un canal sécurisé à la mise à disposition.

---

## Article 5 : Facturation à l'usage

5.1. Sauf forfait précisé au Devis, le Service est facturé à l'usage, sur la base du volume stocké, du nombre de requêtes et du trafic sortant (egress) constatés sur la période, selon les tarifs indiqués au Devis.

5.2. Le Client est informé que le trafic sortant et les opérations de récupération massive de données peuvent générer une facturation, y compris dans le cadre d'une migration ou d'une réversibilité, sous réserve des conditions de l'article 9 des CGV.

---

## Article 6 : Durabilité, redondance et protection des données

6.1. LaMeDuSe assure la durabilité et la redondance des données stockées au sein de la plateforme, par la réplication de chaque objet sur plusieurs supports, afin de préserver l'intégrité des données contre la défaillance d'un support matériel. Cet engagement de durabilité relève de la responsabilité de LaMeDuSe et est inclus dans le Service de base.

6.2. Cette durabilité ne constitue pas une sauvegarde et ne protège pas contre une suppression, un écrasement ou une altération des objets résultant d'une action du Client, de ses applications ou des tiers qu'il autorise. La protection contre de telles actions relève des fonctionnalités de versioning et de verrouillage d'objet (object-lock), que le Client active et configure, ou des options souscrites au Devis.

6.3. Le Client demeure responsable de la gestion des versions, du cycle de vie et des règles de rétention de ses objets, ainsi que, le cas échéant, de la constitution d'une copie de ses données en dehors du Service à des fins de reprise après sinistre logique.

---

## Article 7 : Niveau de service (SLA)

7.1. LaMeDuSe garantit, pour l'infrastructure de stockage relevant de sa responsabilité, un taux de disponibilité mensuel qui dépend de la **gamme de service** souscrite et précisée au Devis (**99,9 %** pour la gamme Essentiel, **99,95 %** pour la gamme Avancé, **99,99 %** pour la gamme Critique), mesuré sur une base mensuelle glissante, dans les conditions et exclusions prévues à l'article 12 des CGV et à l'annexe SLA. À défaut d'indication de gamme au Devis, la gamme Essentiel (99,9 %) s'applique.

7.2. Ce SLA porte sur la disponibilité du point d'accès au Service. Il ne couvre pas les indisponibilités résultant des applications, configurations, clés ou manipulations du Client, ni de son propre réseau d'accès.

---

## Article 8 : Responsabilités du Client

8.1. Le Client est seul responsable :
   - de la gestion et de la confidentialité de ses clés d'accès, ainsi que des droits qu'il accorde à des tiers ou à ses applications ;
   - du contenu des objets qu'il stocke et de leur conformité à la réglementation applicable et à l'AUP prévue à l'article 14 des CGV ;
   - de la gestion du versioning, du cycle de vie et des règles de rétention de ses objets, et de la protection contre ses propres suppressions ou altérations, la durabilité de la plateforme relevant de LaMeDuSe conformément à l'article 6 ;
   - de la configuration des accès publics ou privés à ses buckets, LaMeDuSe ne pouvant être tenue responsable d'une exposition de données résultant d'une configuration ouverte décidée par le Client.

8.2. Le Client garantit LaMeDuSe contre toute conséquence dommageable résultant d'un contenu illicite stocké ou d'un défaut de configuration des accès dont il a la charge.

---

## Article 9 : Suspension et résiliation

9.1. En cas de manquement du Client à ses obligations (impayé, usage abusif, contenu illicite, signalement d'abus non traité), LaMeDuSe applique les modalités de suspension prévues aux articles 14.4 et 18 des CGV et à l'AUP.

9.2. La résiliation du Service par le Client s'effectue avec un préavis de **trente (30) jours calendaires** avant la fin de la période de facturation en cours, sauf disposition contraire au Devis.

---

## Article 10 : Sort des données en fin de contrat

10.1. Il appartient au Client d'avoir extrait, avant la date d'effet de la résiliation ou de l'expiration du Service, l'ensemble de ses objets, au moyen de l'API S3 ou des outils compatibles.

10.2. La restitution et la suppression des Données s'effectuent dans les conditions de réversibilité de l'article 9 des CGV, la période de conservation de **trente (30) jours** prévue à l'article 9.2 des CGV s'appliquant, sauf disposition contraire au Devis. Les coûts de trafic sortant liés à une extraction massive sont supportés par le Client dans les conditions de l'article 9.1 des CGV.

---

## Article 11 : Obligation légale d'identification (LCEN)

Conformément au V de l'article 6 de la loi n° 2004-575 du 21 juin 2004 pour la confiance dans l'économie numérique (LCEN), dans sa rédaction issue de la loi n° 2024-449 du 21 mai 2024, et à l'article L. 34-1 du Code des postes et des communications électroniques, LaMeDuSe, en sa qualité de fournisseur de services d'hébergement, détient et conserve les données de nature à permettre l'identification des contributeurs aux contenus, dans les conditions de l'article 19 des CGV. Le Client s'engage à fournir des informations d'identification exactes et à jour, conformément à l'article 6 des CGV.

---

## Article 12 : Articulation avec les CGV

Pour tout point non expressément traité par les présentes CP (facturation, responsabilité, données personnelles, force majeure, résiliation pour manquement, droit applicable, juridiction compétente), les dispositions des CGV Hébergement LaMeDuSe s'appliquent pleinement et sans réserve.

---

*Dernière mise à jour : 16 juillet 2026*
