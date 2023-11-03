# Titre de la compétence

> ❌ A travailler

> ✔️ Auto validation par l'étudiant

## 🎓 J'ai compris et je peux expliquer

- l'état (_state_) pour contrôler l'affichage d'un composant  ✔️
- les composants enfants et les _props_ qu'on leur passe ✔️
- le déclenchement d'instructions en fonction des actions de l'utilisateur ✔️
- le déclenchement d'instructions en fonction de l'étape du cycle de vie du composant ou du changement de valeur de ses props  ✔️
- l'usage d'un reducer (_useReducer_) pour gérer un état composé dans un composant
- l'état stocké dans un composant avec un _context provider_ et accessible dans ses descendants via `useContext` ✔️

## 💻 J'utilise

### Un exemple personnel commenté  ✔️
Le  code ci-dessous est réalisé en REACT il a pour fonction d'afficher du texte ainsi que des images.
`
// Import de la librairie React
import React from "react";
// Import de l'image nommé logoFeuilleTitle
import logoFeuilleTitle from "../../../assets/logoFeuille.png"
// Import de l'image nommé logoFeuilleTitleDown
import logoFeuilleTitleDown from "../../../assets/logoFeuille.png"
// Déclaration de la fonction HomePageSectionPresentation
function HomePageSectionPresentation(){
// Mise en place du JSX
    return(
        // Ajouter des balises div afin d'encapsuler le code et ajouter des classNames afin de personnaliser les feuilles de styles
        <div className="container">
        <div className="title-content">
        // Ajout de la balise affichant l'image
        <img src= {logoFeuilleTitle} alt="logoFeuille" className="logoImage" />
        // Ajout de la balise affichant un titre secondaire
    <h2 className="title">Are you <span className="highlighted">ready</span> to faces the challenges?</h2>
    </div>
    // Ajouter des balises div afin d'encapsuler le code 
    <div className="container-text">
    // Ajouter de la balise p afin d'ajouter un contenu de type paragraphe
    <p className="description">Join our <span className="highlighted">echo-challenge app</span> and participate in group challenges tant promotes
        substainable actions to support the environment. Together, let's accomplish various eco-friendly
        gestures and make a difference for a better world !<br />
    </p>
    / Ajout de la balise affichant l'image
    <img src= {logoFeuilleTitleDown} alt="logoFeuille" className="logoImageDown" />
    </div>
    Ajouter de la balise span afin d'ajouter un contenu de type texte en une ligne
    <span className="hashtag"> #Ecochallenge #SupportingTheEnvironnement</span>
    </div>
    )
}
// Export de la classe HomePageSectionPresentation afin de pouvoir l'appeler dans d'autre fichiers.
export default HomePageSectionPresentation;
`
### Utilisation dans un projet ❌ / ✔️

[lien github](...) https://github.com/AnkaPieka/ecogeste/blob/US14-Section_Pr%C3%A9sentation/Home_Page-Section_Pr%C3%A9sentation/front/src/Pages/HomePage.tsx

Description : J'ai notamment utiliser React dans la mise de l'affichage de la page principale. Nous avons décidé d'utiliser une structure atomique nous avons créé des composants réutilisables et nous les avons appelés dans notre fichier HomePage.tsx afin de les afficher dans l'ordre voulu.

### Utilisation en production si applicable❌ / ✔️

[lien du projet](...)

Description :

### Utilisation en environement professionnel ❌ / ✔️

Description :

## 🌐 J'utilise des ressources

### Titre

- lien
- description
- React est la documentation officiel, elle indique les informations nécessaires afin de créer une  web app en React  on peut y trouver  la défintion de l'ensemble des concepts tels que JSX, les React Hook avec les useState et les useReducer,  des tutoriels et des blogs...
https://fr.react.dev/learn
- MDN est une document délibrant énormément d'informations sur JavaScript et également sur React, elle indique quels sont ce cas d'utilisateur, comment configurer une application React et commment React utilise JavaScript...
https://developer.mozilla.org/fr/docs/Learn/Tools_and_testing/Client-side_JavaScript_frameworks/React_getting_started
- vidéos: Visualisation des vidéos de Grafikart qui introduit aux notions fondamentales de React:
https://www.youtube.com/watch?v=NT0s0aOHu0Q&ab_channel=Grafikart.fr


## 🚧 Je franchis les obstacles

### Point de blocage ❌ / ✔️

Description:

Plan d'action : (à valider par le formateur)

- action 1 ❌ / ✔️
- action 2 ❌ / ✔️
- ...

Résolution :

## 📽️ J'en fais la démonstration

- J'ai ecrit un [tutoriel](...) ❌ / ✔️
- J'ai fait une [présentation](...) ❌ / ✔️
