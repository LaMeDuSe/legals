# Conditions Particulières : Service de Stockage NAS (Fichier Réseau)

**LaMeDuSe SAS**

---

## Préambule

Les présentes Conditions Particulières (ci-après les « **CP** ») complètent et précisent les Conditions Générales de Vente Services d'Hébergement de LaMeDuSe SAS (ci-après les « **CGV** ») pour ce qui concerne spécifiquement le service de **stockage fichier en réseau (NAS)** (ci-après le « **Service** »).

Conformément à l'article 37.3 des CGV, en cas de contradiction entre les documents contractuels, l'ordre de priorité suivant s'applique : (i) le Devis ou Bon de Commande, (ii) les présentes CP, (iii) les CGV, (iv) les autres annexes. Pour tout point non traité par les présentes CP, les dispositions des CGV s'appliquent pleinement.

---

## Article 1 : Objet

Les présentes CP ont pour objet de définir les conditions spécifiques applicables à la fourniture par LaMeDuSe d'un service de stockage fichier en réseau (NAS, *Network Attached Storage*), accessible en partage via des protocoles réseau standards, dans les conditions décrites au Devis.

---

## Article 2 : Définitions spécifiques

- **NAS (stockage fichier réseau)** : espace de stockage partagé, accessible sous forme de système de fichiers via des protocoles réseau standards (par exemple NFS ou SMB/CIFS), selon les options du Devis.
- **Partage (share)** : espace logique du NAS exposé au Client, soumis à des règles d'accès qu'il définit.
- **Point de montage** : ressource réseau permettant à une instance de calcul ou à un poste autorisé d'accéder au partage.
- **Protocole d'accès** : protocole réseau (NFS, SMB/CIFS ou équivalent) mis à disposition pour l'accès au partage, précisé au Devis.

---

## Article 3 : Description du Service et localisation

3.1. Le Service met à disposition du Client un espace de stockage fichier partagé, dont la capacité, le ou les protocoles d'accès et les performances sont précisés au Devis.

3.2. Le partage est accessible depuis les instances de calcul ou les ressources autorisées par le Client, via le réseau interne de LaMeDuSe ou, lorsque le Devis le prévoit, via un accès sécurisé dédié. Le Client définit les règles d'accès à ses partages.

3.3. Le Service assure la durabilité et la redondance des données au sein de la plateforme : les données sont réparties de manière redondante par LaMeDuSe, de façon à préserver leur intégrité contre la défaillance d'un support matériel. Cette redondance ne constitue pas une protection contre les erreurs du Client au sens de l'article 5 des présentes CP.

3.4. Le Service est hébergé dans un Datacenter situé en **France, en Allemagne ou en Suisse**, la localisation retenue étant indiquée au Devis, conformément à l'article 4 des CGV.

---

## Article 4 : Commande et mise à disposition

4.1. Toute commande fait l'objet d'un Devis précisant la capacité, le ou les protocoles d'accès, les performances et le tarif applicable.

4.2. Le Service est provisionné de manière automatisée. LaMeDuSe communique au Client les informations d'accès (points de montage, paramètres de connexion) par un canal sécurisé.

---

## Article 5 : Durabilité, redondance et instantanés

5.1. LaMeDuSe assure la durabilité et la redondance des données stockées sur le NAS au sein de la plateforme, afin de préserver leur intégrité contre la défaillance d'un support matériel. Cet engagement de durabilité relève de la responsabilité de LaMeDuSe et est inclus dans le Service de base.

5.2. Cette durabilité ne constitue pas une sauvegarde et ne protège pas contre une suppression, un écrasement ou une altération des fichiers résultant d'une action du Client ou des utilisateurs qu'il autorise. La protection contre de telles actions relève des instantanés (snapshots) et, le cas échéant, d'une option de sauvegarde, que le Client active ou souscrit au Devis, ses modalités (fréquence, durée de rétention, procédure de restauration) étant alors précisées au Devis.

5.3. Il appartient au Client de constituer, le cas échéant, une copie de ses données en dehors du Service à des fins de reprise après une erreur logique de sa part.

---

## Article 6 : Niveau de service (SLA)

6.1. LaMeDuSe garantit, pour l'infrastructure de stockage relevant de sa responsabilité, un taux de disponibilité mensuel qui dépend de la **gamme de service** souscrite et précisée au Devis (**99,9 %** pour la gamme Essentiel, **99,95 %** pour la gamme Avancé, **99,99 %** pour la gamme Critique), mesuré sur une base mensuelle glissante, dans les conditions et exclusions prévues à l'article 12 des CGV et à l'annexe SLA. À défaut d'indication de gamme au Devis, la gamme Essentiel (99,9 %) s'applique.

6.2. Ce SLA porte sur la disponibilité du Service et de son accessibilité réseau au sein de l'infrastructure de LaMeDuSe. Il ne couvre pas les indisponibilités résultant des instances ou postes du Client, de leur système d'exploitation, des configurations d'accès, ou du réseau d'accès propre au Client.

---

## Article 7 : Responsabilités du Client

7.1. Le Client est seul responsable :
   - de la définition et de la gestion des droits d'accès à ses partages, ainsi que des utilisateurs et instances qu'il autorise ;
   - de la cohérence des accès concurrents à ses fichiers ;
   - de la protection contre ses propres suppressions ou altérations de fichiers, au moyen des instantanés ou d'une option de sauvegarde, la durabilité de la plateforme relevant de LaMeDuSe conformément à l'article 5 ;
   - du contenu stocké et de sa conformité à la réglementation applicable et à l'AUP prévue à l'article 14 des CGV.

7.2. Le Client garantit LaMeDuSe contre toute conséquence dommageable résultant d'un contenu illicite stocké ou d'une configuration d'accès dont il a la charge.

---

## Article 8 : Suspension et résiliation

8.1. En cas de manquement du Client à ses obligations (impayé, usage abusif, contenu illicite, signalement d'abus non traité), LaMeDuSe applique les modalités de suspension prévues aux articles 14.4 et 18 des CGV et à l'AUP.

8.2. La résiliation du Service par le Client s'effectue avec un préavis de **trente (30) jours calendaires** avant la fin de la période de facturation en cours, sauf disposition contraire au Devis.

---

## Article 9 : Sort des données en fin de contrat

9.1. Il appartient au Client d'avoir réalisé, avant la date d'effet de la résiliation ou de l'expiration du Service, l'ensemble des sauvegardes et exports des données présentes sur le NAS. À la date d'effet de la résiliation, l'accès aux partages est coupé.

9.2. La restitution et la suppression des Données s'effectuent dans les conditions de réversibilité de l'article 9 des CGV, la période de conservation de **trente (30) jours** prévue à l'article 9.2 des CGV s'appliquant, sauf disposition contraire au Devis. Passé ce délai, l'espace est effacé de manière sécurisée et remis en disponibilité.

---

## Article 10 : Obligation légale d'identification (LCEN)

Conformément au V de l'article 6 de la loi n° 2004-575 du 21 juin 2004 pour la confiance dans l'économie numérique (LCEN), dans sa rédaction issue de la loi n° 2024-449 du 21 mai 2024, et à l'article L. 34-1 du Code des postes et des communications électroniques, LaMeDuSe, en sa qualité de fournisseur de services d'hébergement, détient et conserve les données de nature à permettre l'identification des contributeurs aux contenus, dans les conditions de l'article 19 des CGV. Le Client s'engage à fournir des informations d'identification exactes et à jour, conformément à l'article 6 des CGV.

---

## Article 11 : Articulation avec les CGV

Pour tout point non expressément traité par les présentes CP (facturation, responsabilité, données personnelles, force majeure, résiliation pour manquement, droit applicable, juridiction compétente), les dispositions des CGV Hébergement LaMeDuSe s'appliquent pleinement et sans réserve.

---

*Dernière mise à jour : 16 juillet 2026*
