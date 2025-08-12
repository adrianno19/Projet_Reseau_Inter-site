# Projet : Interconnexion de deux sites avec routage hybride et services réseau essentiels

## Description du Projet 🌐

Ce projet présente l'interconnexion de deux sites distincts en utilisant une topologie de routage hybride. L'objectif principal était de garantir une communication fluide et sécurisée entre les différents réseaux (VLANs) de chaque site, tout en intégrant des services essentiels pour les utilisateurs finaux.

* **Site 1 : Routage Inter-VLAN via "Router on a stick"**
    Ce site a été configuré pour gérer le trafic inter-VLAN en utilisant une seule interface physique d'un routeur, subdivisée en sous-interfaces logiques. Cette méthode est efficace pour les topologies où le nombre de ports de routeur est limité.

* **Site 2 : Routage Inter-VLAN via Switch de niveau 3**
    Ce site utilise un switch de niveau 3 qui gère nativement le routage inter-VLAN. Cette approche est plus performante et scalable, car elle s'appuie sur le matériel (ASIC) pour le routage, évitant ainsi un goulot d'étranglement.

## Interconnexion et Services Réseau 🔗

Les deux sites sont reliés par un **lien de routage statique** entre les deux routeurs principaux. Pour simuler un environnement de production, les services suivants ont été mis en place :

* **Serveurs DHCP :** Configuration de serveurs DHCP sur chaque site pour l'attribution automatique d'adresses IP. Le relais DHCP est configuré sur les passerelles pour garantir que les requêtes soient acheminées correctement.
* **Serveurs DNS :** Mise en place de serveurs DNS pour la résolution de noms de domaine, permettant une navigation plus aisée.
* **Serveurs Web :** Déploiement de serveurs Web pour tester la connectivité et la résolution de noms entre les différents sites et VLANs.

## Technologies et Compétences 🛠️

* **Matériel :** Cisco Packet Tracer
* **Configuration :** Cisco IOS
* **Protocoles :** VLANs, Trunking (802.1Q), Routage Statique, DHCP, DNS, IP (IPv4)
* **Méthodes :** Router on a stick, Routage inter-VLAN sur Switch L3, Relais DHCP.

## Topologie du Réseau

Pour une meilleure compréhension de l'architecture, la topologie du réseau est disponible.


---

### Comment utiliser ce dépôt

Ce dépôt contient les fichiers de configuration de tous les équipements du projet. Vous pouvez les utiliser pour reproduire la topologie et la configuration dans Cisco Packet Tracer.
