# 👋 Bonjour, je suis Ch3rch3ur

## 🔧 Administrateur Systèmes & Réseaux

Titulaire d'un **BTS CIEL option IR**, je poursuis une montée en compétences en administration systèmes et réseaux à travers des projets personnels documentés. Mon expertise couvre l'administration système, la virtualisation, la sécurité réseau et l'intégration d'environnements Windows/Linux en contexte professionnel.

📍 **France** | 📫 [GitHub](https://github.com/Ch3rch3ur) | [Portfolio](https://professionnel.hopto.org) | [LinkedIn](https://linkedin.com/in/joris-godard-ba85b1350/)

---

## 💼 Compétences Techniques

| Catégorie          | Technologies/Outils                                                                 |
|--------------------|------------------------------------------------------------------------------------|
| **Systèmes**       | Debian, Linux Mint, Kali Linux, Raspberry Pi OS, Windows Server 2022             |
| **Réseaux**        | Cisco (switches/routeurs - partiqué en formation), pfSense, WireGuard, TCP/IP, DNS (A/PTR/SRV), DHCP, VLAN, NAT, Firewall    |
| **Virtualisation** | VirtualBox, Active Directory                                         |
| **Scripting**      | Bash, Python, PowerShell                                                           |
| **Services**       | Apache, VPN, Kerberos, SSSD, PAM, NSS, DNS                                 |
| **Sécurité**       | Let's Encrypt, HTTPS, UFW, Headers HTTP (CSP, HSTS, X-Frame-Options)             |
| **Authentification** | Active Directory, Kerberos, LDAP, Gestion des privilèges                        |
| **En apprentissage** | Monitoring (Zabbix, Prometheus), Automatisation (Ansible, Terraform)            |

---

## 🚀 Projets Personnels

Je développe des projets qui reproduisent des **scénarios réalistes d'entreprise** pour consolider mes compétences techniques. Chaque projet est documenté avec architecture, problèmes rencontrés et solutions apportées.

### 📌 Projets en Vedette

#### 🔐 [Intégration Linux ↔ Active Directory](https://github.com/Ch3rch3ur/Projets-personnelles/tree/main/Projet-ActiveDirectory-Debian)
Authentification centralisée Active Directory pour systèmes Linux Debian
- Intégration complète de clients Debian dans un domaine Active Directory
- Authentification centralisée via **Kerberos** (KDC Windows Server)
- Gestion des identités et groupes via **SSSD**
- Contrôle d'accès SSH par groupes AD : `linux-users` (accès SSH) et `linux-admins` (SSH + sudo)
- Résolution DNS complète (A, PTR, SRV)
- Création automatique des home directories via PAM
- Aucune solution propriétaire tierce, compréhension approfondie des mécanismes
- **Stack:** Windows Server 2022 (AD DS, DNS, Kerberos), Debian, SSSD, PAM, NSS, Kerberos

#### 🏠 [Homelab Virtualisé avec pfSense](https://github.com/Ch3rch3ur/Projets-personnelles/tree/main/Projet-Homelab-pfSense)
Infrastructure multi-OS complète simulant un réseau d'entreprise
- Infrastructure réseau virtualisée sous **VirtualBox** sur Kali Linux
- Pare-feu **pfSense** dédié avec segmentation LAN/WAN
- Machines virtuelles : Debian, Windows Server 2022 (évaluation 180 jours)
- NAT configuré malgré contrainte d'une seule carte réseau physique
- Configuration manuelle des interfaces réseau via `VBoxManage`
- Réseau isolé du réseau local principal
- **Stack:** VirtualBox, pfSense, Windows Server 2022, Debian, Kali Linux

#### 🔒 [VPN Personnel WireGuard](https://github.com/Ch3rch3ur/Projets-personnelles/tree/main/Projet-VPN-WireGuard)
Déploiement d'un VPN sécurisé sur Raspberry Pi pour accès distant
- Serveur VPN **WireGuard** hébergé sur **Raspberry Pi 5**
- Installation via **PiVPN** avec configuration du routage et NAT
- Support multi-clients (PC, smartphone) avec connexion via QR code
- Activation du forwarding IP et routage réseau
- Pare-feu **UFW** configuré avec politique restrictive
- Résolution de blocage firewall sur le trafic VPN (port UDP 51820, règles de routage)
- Accès distant sécurisé aux ressources locales et connexion chiffrée en mobilité
- **Stack:** WireGuard, PiVPN, Raspberry Pi OS, UFW, NAT

#### 🌐 [Portfolio Web Apache Sécurisé](https://github.com/Ch3rch3ur/Projets-personnelles/tree/main/Projet-Serveur-Web-Apache)
Hébergement d'un portfolio personnel avec sécurisation complète
- Serveur web **Apache** hébergé sur **Raspberry Pi 5**
- Portfolio personnel accessible publiquement : [professionnel.hopto.org](https://professionnel.hopto.org)
- HTTPS avec certificats **Let's Encrypt** (renouvellement automatique)
- IP dynamique gérée via **No-IP**
- Durcissement du serveur avec headers de sécurité : HSTS, CSP, X-Frame-Options
- Résolution de politique CSP trop restrictive bloquant les ressources (Tailwind CSS)
- Arbitrage entre sécurité et fonctionnalité
- **Stack:** Apache, Let's Encrypt, Raspberry Pi OS, No-IP, HTTPS

---

## 🔄 Prochaines étapes

- 📝 **Documentation complète** de mes configurations et procédures sur GitHub
- 🖥️ **Intégration de machines Windows** supplémentaires à l'Active Directory
- 📊 **Mise en place d'outils de monitoring** (Zabbix/Prometheus) pour supervision d'infrastructure
- 🤖 **Automatisation des déploiements** avec Ansible et Terraform
- 🔐 **Centralisation des logs** et exploitation pour améliorer la sécurité

---

## 🏗️ Architecture de mon Homelab

Mon environnement de test reproduit une infrastructure d'entreprise complète :

- **Pare-feu pfSense** : Segmentation réseau LAN/WAN, règles de filtrage, contrôle des flux
- **Windows Server 2022** : Active Directory, DNS (A/PTR/SRV), DHCP, Kerberos KDC
- **Clients Linux** : Debian (intégré au domaine AD), Kali Linux (hôte de virtualisation)
- **VPN WireGuard sur Raspberry Pi 5** : Accès distant sécurisé avec pare-feu UFW
- **Serveur Web Apache sur Raspberry Pi 5** : Portfolio public HTTPS avec headers de sécurité

Cette infrastructure me permet de :
- Simuler des scénarios d'entreprise réalistes
- Tester l'intégration Windows/Linux
- Appliquer des bonnes pratiques de sécurité réseau
- Développer mes compétences en conditions proches de la production

---

## 🎯 Objectifs

- Consolider mes compétences en administration systèmes et réseaux
- Me préparer à une **licence professionnelle Administrateur Systèmes & Réseaux**
- Comprendre les mécanismes sous-jacents au-delà du "clé en main"
- Apprendre les bonnes pratiques professionnelles (sécurité, maintenance, documentation)
- Partager mes expériences et retours d'expérience avec la communauté

---

## 📊 Statistiques GitHub

![GitHub Stats](https://github-readme-stats.vercel.app/api?username=Ch3rch3ur&show_icons=true&theme=dark)

---

## 💬 À Propos

Je documente mes projets et mes apprentissages sur GitHub pour laisser une trace de mon évolution technique. Chaque projet inclut :
- Architecture détaillée avec schémas réseau
- Problèmes rencontrés et solutions apportées
- Scripts et fichiers de configuration
- Compétences démontrées et améliorations possibles

Ces projets reproduisent des scénarios professionnels : authentification centralisée, sécurité réseau, séparation des privilèges, et exposition de services en production.

📎 Mon profil évolue régulièrement avec l'ajout de nouvelles fonctionnalités et documentation.

---

💡 *En constante évolution, toujours à la recherche de nouveaux défis techniques.*
