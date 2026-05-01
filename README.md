# Web Application Security Audit Lab 

## Domaine choisi
Sécurité Informatique

## Problème traité
Ce projet consiste en un mini-audit de sécurité réalisé sur 
OWASP Juice Shop, une application web volontairement vulnérable.
L'objectif est d'identifier, comprendre et documenter des 
failles de sécurité courantes, puis proposer des corrections.

## Outils utilisés
- Kali Linux
- OWASP Juice Shop v17.1.1
- Node.js v22.22.2
- Firefox
- Git

## Installation

### Prérequis
- Kali Linux
- Node.js installé

### Lancer le projet
>>>bash
cd juice-shop_17.1.1
node build/app

Ouvrir Firefox et aller sur : http://localhost:3000
Failles documentées
#                   faille                    risque
1               injection SQL                 Elévé
2            XCC(Cross-Site Scripting         Elévé
3            Authentification cassée          Elevé
4            Exposition de données sensible   Elévé

##Le rapport détaillé est disponible dans le dossier /docs
Captures d'écran
##Disponibles dans le dossier /screenshots

###Difficultés rencontrées
+Configuration du réseau WiFi sur Kali Linux
+Problèmes de timeout lors de l'installation via npm

###Solution : 
-utilisation de la version pré-compilée de Juice Shop

###Améliorations possibles
+Tester davantage de failles (CSRF, broken access control)
+Utiliser OWASP ZAP pour un scan automatique
+Tester avec Burp Suite

###Ce que j'ai appris
-Comment fonctionne une injection SQL
-Comment fonctionne une attaque XSS
-L'importance des questions secrètes comme mauvaise pratique
-Les risques liés à l'exposition de fichiers sensibles
-L'utilisation de Kali Linux pour la cybersécurité
