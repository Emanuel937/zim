# AutoCompiler Script

**Auteur : Emanuel Abizimi**

## Description

`AutoCompiler` est un script Bash conçu pour surveiller les modifications d'un fichier spécifique et redémarrer automatiquement le processus de compilation ou d'exécution avec le compilateur ou interpréteur spécifié. Cet outil est utile pour les développeurs travaillant dans des langages comme PHP, Python, ou d'autres, où les fichiers sources doivent être rechargés fréquemment.

---

## Fonctionnalités

- Surveillance en continu des modifications d'un fichier donné.
- Redémarrage automatique du processus lorsque le fichier est mis à jour.
- Supporte n'importe quel compilateur ou interpréteur (ex. : PHP, Python, etc.).
- Gestion des erreurs en cas de fichier inexistant ou d'arguments incorrects.

---

## Pré-requis

- Système d'exploitation Linux ou macOS avec Bash.
- Accès à un interpréteur ou compilateur pour le langage cible (ex. : PHP 8, Python 3, etc.).

---

## Installation

1. Téléchargez le script et assurez-vous qu'il est exécutable :
   ```bash
   chmod +x AutoCompiler.sh
