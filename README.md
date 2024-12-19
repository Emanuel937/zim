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
   chmod +x zim



# AutoCompiler Script - Structure et Détails

## Structure du Code

Le script est structuré de manière à exécuter plusieurs tâches essentielles pour surveiller un fichier et redémarrer un processus de compilation ou d'exécution lorsque le fichier est modifié. Voici les principales parties du script :

1. **Vérification des arguments** :
   - Valide les arguments fournis lors de l'exécution du script.
   - S'assure que les bons paramètres sont passés pour le fichier source et le compilateur/interpréteur.

2. **Surveillance des modifications** :
   - Utilise la commande `stat` pour vérifier les changements dans la date de modification du fichier.
   - Permet de détecter les changements dans le fichier source afin de savoir s'il faut redémarrer le processus.

3. **Gestion des processus** :
   - Lance le compilateur ou interpréteur pour le fichier spécifié, par exemple en exécutant `php8` ou `python3` en fonction de l'argument fourni.
   - Si une modification est détectée, le processus actuel est redémarré pour utiliser la version mise à jour du fichier.

4. **Boucle infinie** :
   - Le script continue de surveiller le fichier dans une boucle infinie.
   - Il effectue des vérifications toutes les secondes (par défaut) pour détecter d'éventuelles modifications.

---

## Limitations

Bien que ce script soit utile dans de nombreux cas, il présente certaines limitations :

1. **Compatibilité** :
   - Le script utilise des commandes spécifiques à Linux/macOS comme `stat` et `kill`, ce qui pourrait limiter sa compatibilité avec des systèmes comme Windows.
   
2. **Cas complexes non gérés** :
   - Le script ne gère pas les cas complexes comme les dépendances multiples entre fichiers ou les fichiers inclus dans le fichier surveillé.

---

## Contribution

Les contributions sont les bienvenues ! Si vous trouvez des bugs ou souhaitez ajouter des fonctionnalités, n'hésitez pas à :

- Soumettre une pull request
- Ouvrir une issue

Nous encourageons les utilisateurs à améliorer le script en proposant des améliorations ou des corrections de bugs.

---

## Licence

Ce projet est distribué sous la licence [MIT](LICENSE).

