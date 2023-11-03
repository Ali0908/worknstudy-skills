# Titre de la compétence

> ❌ A travailler

> ✔️ Auto validation par l'étudiant

## 🎓 J'ai compris et je peux expliquer

- les différences et points communs entre du code react et du code react native  ✔️
- ce que devient et comment est interprêté le code javascript dans une application react native  ✔️
- les avantages et inconvénients de react native ✔️
- la différence entre react native et expo ✔️
- les principales briques qui composent react native (core components)  ✔️
- comment écrire du style en react native  ✔️
- comment est géré le layout en react native ✔️

## 💻 J'utilise

### Un exemple personnel commenté ✔️
 L'objectif du code ci-dessous est d'afficher la page d'acceuil de mon application, celle-ci contient une image des titres de différentes tailles, un bouton intitulé commencer permettant d'accéder à la page de connexion ou d'inscription.
 // Déclaration d'une nouvelle fonction
export default function StartScreen({ navigation }) {
// Chargement de la police à afficher
  const [loaded] = useFonts({
    Karma: require("../../assets/fonts/Karma/Karma-Regular.ttf"),
  });

  if (!loaded) {
    return null;
  }

  return (
// Déclaration d'une balise englobant l'ensemble du code et import des fichiers de style
    <View style={[global.container, styles.font]}>
// Déclaration de la balise permettant de contenir une image et import des fichiers de style
      <Image
        source={require("./../../assets/earth-logo.png")}
        style={[global.imageResize, styles.logo]}
      />
// Déclaration d'une balise englobant les titres et le bouton  et import des fichiers de style
      <View style={[styles.textAndBtnContainer]}>

// Déclaration de la balise contenant le titre principal
        <Text
          style={[
            global.colorWhite,
            global.h1,
            styles.font,
            styles.title,
            styles.titleBottomBorder,
          ]}
        >
          Eco Challenge
        </Text>

// Déclaration de la balise contenant le titre secondaire
        <Text style={[global.colorWhite, global.h4, styles.font, styles.subTitle]}>
          Êtes-vous de taille à relever le défi ?
        </Text>

// Déclaration de la balise de type bouton permettant d'accéder à la page d'inscription/connexion
        <Pressable
          style={[global.button, styles.startButton]}
          onPress={() => navigation.navigate("Login")}
        >
          <Text style={[global.colorPurple, styles.font, styles.startButtonText]}>
            Commencer
          </Text>
        </Pressable>
      </View>
    </View>
  );
}

### Utilisation dans un projet ❌ / ✔️

[[lien github](...)](https://github.com/AnkaPieka/ecogeste-mobile)

Description : Application écogeste codée en React Native offrant à ses utilisateurs la possibilité de créer des challenges écologiques en se créant son compte sur la plateforme.

### Utilisation en production si applicable❌ / ✔️

[lien du projet](...)

Description :

### Utilisation en environement professionnel ❌ / ✔️

Description :

## 🌐 J'utilise des ressources

### Titre

- lien
- description
- React Native documentation: https://reactnative.dev/docs/getting-started
React Native est la documentation officiel, elle permet d'otenir l'ensemble des informations nécessaires afin de créer une app en React Native on peut y trouver  la défintion de l'ensemble des conceptes tels que les Core Components contenant notamment les balises View, Text et Image,  des tutoriels et des blogs...

Github: https://github.com/facebook/react-native
Indication sur la démarche à suivre afin d'installer React Native sur Windows, macOS, or Linux. On trouve  notamment dessus les différentes versions de React Native ainsi qu'un tutoriel afin de créer sa première application sur React Native

React Native vidéos: Meta le fondateur de React a mis à disposition sur YouTube une série de vidéos sur React Native, j'ai consulté les vidéos concernant React.js Conf 2015 Keynote - Introducing React Native dans laquelle le groupe explique les raisons qui les ont poussés à créer ce logiciel.
https://www.youtube.com/watch?v=KVZ-P-ZI6W4&ab_channel=MetaDevelopers

## 🚧 Je franchis les obstacles

### Point de blocage ❌ / ✔️

Description:
J'ai rencontré un souci dans l'affichage de l'avatar sur la page d'inscription.

Plan d'action : (à valider par le formateur)

- action 1 ❌ / ✔️
- action 2 ❌ / ✔️
- ...
- action 1: Relecture de la documentation de React Native.
- action 2: Recherche sur divers plateformes comme StackOverflow
- action 3: Sollicitations de mes collègues

Résolution :

J'ai trouvé un code similaire au mien, j'ai dus ajouter une interface et ajouter une méthode afin de gérer la gestion de l'ouverture ou fermeture d'une fenêtre modal. 

## 📽️ J'en fais la démonstration

- J'ai ecrit un [tutoriel](...) ❌ / ✔️
- J'ai fait une [présentation](...) ❌ / ✔️
