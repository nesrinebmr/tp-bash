
# Réponses aux questions de réflexion

## Exercice 2.1
La commande chmod 644 attribue les permissions rw-r--r-- :
le propriétaire peut lire et écrire, tandis que le groupe et
les autres utilisateurs peuvent uniquement lire. Le propriétaire
ne peut donc pas exécuter le fichier.

## Exercice 2.2
Les guillemets autour de "$UTILISATION" protègent la valeur de la
variable et évitent les problèmes d'interprétation. Ils permettent
de transmettre la valeur comme un seul argument au test numérique.

## Exercice 2.3
Sans set -Eeuo pipefail, le script peut continuer après certaines
erreurs si elles ne sont pas vérifiées. L'option -e arrête le script
dans de nombreux cas d'échec, -u détecte les variables non définies,
pipefail détecte les échecs dans les pipelines et -E transmet
l'héritage des pièges ERR dans certains contextes.

## Exercice 2.4
Cron utilise un environnement différent du terminal, avec un
répertoire courant et des variables d'environnement potentiellement
différents. Les chemins absolus garantissent que les fichiers et
les scripts sont localisés correctement.

## Exercice 2.5
Un vrai pipeline CI peut ajouter l'installation des dépendances,
les vérifications de syntaxe, les tests unitaires et d'intégration,
l'analyse de qualité et de sécurité, la création d'un artefact
et le déploiement. Il faut gérer les erreurs Git, les dépendances
manquantes, les tests échoués, les problèmes de permissions,
les erreurs réseau et les échecs de déploiement.
EOF
