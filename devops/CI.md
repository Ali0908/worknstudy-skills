# Integration continue

> ❌ A travailler

> ✔️ Auto validation par l'étudiant

## 🎓 J'ai compris et je peux expliquer

- les enjeux de l'integration continue ✔️
- la mise en place d'une github action  ✔️

## 💻 J'utilise

### Un exemple personnel commenté ✔️
L'intégration continue est une méthode de développement de logiciel DevOps  permettant aux notamment  développeurs d'intégrer des modifications de code et d'effectuer des tests automatisés.
Voici un exemple de mise en place de CI avec github Actions:
// Nom du workflow
name: client-tests-workflow
// Indication sur l'évènement qui déclenchera le workflow
on: pull_request
// Jobs définit les tâches qui devront être réalisées dans le workflow
jobs:
// test-client indique le nom du job
  test-client:
// runs-on indique l'environnement surlequel ce worflows sera pris en compte. Ce job doit tourner sur la dernière version d'Ubuntu.
    runs-on: ubuntu-latest
// On liste les étapes contenus dans notre job
    steps:
// Appel de la première étape 
      - name: Check out code
// Utilisation des actions fournit par Github pour récupérer le code
        uses: actions/checkout@v2
// Appel de la deuxième étape
      - name: Goto client and run tests
// Définition des commandes à lancer dans notre cas, entrer dans le dossier testrunner et lancer l'installation de node package manager ainsi que ses tests.
        run: cd testrunner && npm i && npm test

### Utilisation dans un projet ✔️

https://github.com/AnkaPieka/ecogeste/tree/US-16_CI/.github/workflows

Description : Projet de groupe codée en GraphQl/React  qui est un site permettant aux utilisateurs de créer des challenges écologiques. Le but dans la mise en place de la CI était de vérifier la conformité de l'installation de node package manager ainsi que ses tests.

### Utilisation en production si applicable❌ / ✔️

[lien du projet](...)

Description :

### Utilisation en environement professionnel ❌ / ✔️

Description :

## 🌐 J'utilise des ressources

### Titre

- lien
- description
- Github MarketPlace: https://github.com/marketplace/actions/checkout
- vidéo DEVOPS et CI/CD (avec Github Actions): https://www.youtube.com/watch?v=mhw7eyTA4KQ&ab_channel=inpulsetv
-GitLab: https://docs.gitlab.com/ee/topics/build_your_application.html
## 🚧 Je franchis les obstacles

### Point de blocage ❌ / ✔️

Description:
Après avoir compris les enjeux de l'intégration continue j'ai rencontré un point blocage dans la mise en place d'un wokflow avec Github Actions
Plan d'action : (à valider par le formateur)

- action 1 ❌ / ✔️
- action 2 ❌ / ✔️
- action 1: Recherche active sur internet et notamment sur la documentation officiel de Github afin de comprendre à quoi correspond chaque mot clé: jobs, run, name...
- action 2: Echange avec mes camarades afin d'évoquer les notions qui peuvent être flous tels que le mise en place des steps

Résolution :
Avec l'aide de tutoriels ainsi que celle du formateur, j'ai réussi à comprendre les éléments clés de Github Actions et j'ai réussi à la mettre en place dans mon projet

## 📽️ J'en fais la démonstration

- J'ai ecrit un [tutoriel](...) ❌ / ✔️
- J'ai fait une [présentation](...) ✔️
J'ai fait une présentation de mon workflow à mes camarades sur notre projet chacun des mots clés cités dans l'exemple commenté.