RÉSEAU INTERCONNECTÉ MIKROTIK – CISCO AVEC OSPF, VLAN ET DHCP (GNS3)

📌 DESCRIPTION DU PROJET
************************
Ce projet présente la conception et la mise en œuvre d’un réseau d’entreprise interconnecté basé sur des équipements MikroTik 
et Cisco, simulés dans l’environnement GNS3.

La topologie repose sur une segmentation en VLAN, un routage dynamique OSPF pour l’échange automatique des routes, 
et un service DHCP centralisé sur MikroTik, administré via WinBox et la ligne de commande.

🧩 TOPOLOGIE RÉSEAU
*******************

* Architecture multi-sites (Étage 1 et Étage 2)
* Segmentation par VLAN selon les services
* Interconnexion WAN point-à-point
* Routage inter-VLAN et inter-sites

🌐 PLAN D'ADRESSAGGE
*******************
--- VLAN 10 – ADMIN : 192.168.10.0/24
--- VLAN 20 – SALES : 192.168.20.0/24
--- VLAN 30 – RH : 192.168.30.0/24
--- VLAN 40 – IT : 192.168.40.0/24

Liens WAN :

--- MikroTik ↔ Cisco R1 : 20.0.0.0/30
--- Cisco R1 ↔ Cisco R2 : 10.0.0.0/30

⚙️ FONCTIONNALITÉS MISES EN OEUVRE
**********************************

--- Création et configuration des VLAN
--- Routage inter-VLAN
--- Configuration du protocole OSPF (Area 0)
--- Mise en place d’un serveur DHCP sur MikroTik
--- Distribution automatique des adresses IP aux postes clients
--- Tests de connectivité et de routage
--- Supervision et administration des équipements

🖥️ ADMINISTRATION MIKROTIK (WINBOX)
***********************************

--- L’administration du routeur MikroTik a été réalisée principalement via WinBox, incluant :
--- Configuration des interfaces et des VLAN
--- Mise en place du serveur DHCP
--- Configuration d’OSPF
--- Vérification des routes et des voisins OSPF
--- Surveillance de l’état des interfaces et du trafic

🛠 TECHNOLOGIES ET OUTILS
*************************

--- GNS3
--- MikroTik RouterOS (WinBox & CLI)
--- Cisco IOS
---- OSPF, VLAN, DHCP

📂 CONTENU DU DÉPÔT
*******************

--- Fichier de projet .gns3
--- Schéma de la topologie réseau
--- Captures d’écran (WinBox, CLI Cisco, tests)
--- Documentation (README)

⚠️ Les images système (IOS, qcow2, etc.) ne sont pas incluses volontairement.

✅ VALIDATION
*************

--- OSPF opérationnel sur l’ensemble des routeurs
--- Routes apprises dynamiquement
--- DHCP fonctionnel sur tous les VLAN
--- Communication validée entre les différents services

📅 PÉRIODE
----------
Novembre 2025
