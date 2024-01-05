# Sécurité dans le développement Web

> ❌ A travailler

> ✔️ Auto validation par l'étudiant

## 🎓 J'ai compris et je peux expliquer

- Le rôle de l'OWASP ✔️
 L'OWASP est une ONG dont l'objectif principal est d'assurer la sécurité des application webs. Elle délivre des prestations Open Source, comme des forums, conférences sur les thématiques de la cybersécurité et le classement l'OWASP Top 10 qui indique les injections SQL.
- Les injections SQL  ✔️
- Les injections SQL sont un type d'attaque informatique ou le pirate va hacker les requêtes afin d'en modifier, supprimer, récupérer son contenu.
- XSS  ✔️
- Le XSS indique Cross-Site Scripting correspond à une attaque de sécurité dans laquelle le pirate va injecter des scripts malveillants pour récupérer, modifier ou supprimer des données.
- CRSF  ✔️
Le CSRF Cross-Site Request Forgery également connu sous le nom de XSR est une intrusion dans des applications Webs dans laquelle le pirate va pousser l'utlisateur à éxécuter des actions non désirées. Pour mettre en place cette attaque l'utilisateur doit impérativement être connecté, le pirate peut envoyer un mail frauduleux, si l'utilisateur clique dessus, le hacker pourra accéder à son espace et récupérer ou altérer des données sensibles (compte bancaire).
## 💻 J'utilise

### Un exemple personnel commenté  ✔️
Exemple d'attaque à l'injection SQL:

`function login(username, password) {
  // Dans la requête ci-dessous le paramètre le code est vulnérable car le paramètre username est utilisé directement dans la requête SQL. 
  var query = "SELECT * FROM users WHERE username='" + username + "' AND password='" + password + "'";

// Le pirate peut interférer notre requête est ajouter une condition qui sera toujours vraie, il pourra alors se connecter sans connaître le mot de passe.
  var queryCorrupted = SELECT * FROM users WHERE username='' OR 1=1 --' AND password='" + password + "'";

  var result = db.query(query);

  // Si la requête renvoie un résultat, l'utilisateur est connecté
  if (result.length > 0) {
    return true;
  } else {
    return false;
  }
}`
Afin de prémunir de l'attaque il faut encoder  la chaîne username avant de l'utiliser dans la requête SQL
`
// Récupération de la  la bibliothèque mysql de Node.js qui fournit la fonction escape() pour encoder les données sensibles.
const mysql = require("mysql");

function login(username, password) {
  // Encodage de la chaîne username
  const encodedUsername = mysql.escape(username);

  // Exécuter une requête SQL pour vérifier les informations de connexion
  const query = "SELECT * FROM users WHERE username='" + encodedUsername + "' AND password='" + password + "'";
  const result = db.query(query);

  // Si la requête renvoie un résultat, l'utilisateur est connecté
  if (result.length > 0) {
    return true;
  } else {
    return false;
  }
}`

### Utilisation dans un projet ❌ / ✔️

[lien github](...)

Description :

### Utilisation en production si applicable❌ / ✔️

[lien du projet](...)

Description :

### Utilisation en environement professionnel ❌ / ✔️

Description :

## 🌐 J'utilise des ressources

### Titre

- lien
- description

OWASP: https://owasp.org/ : Site officiel de Open Worldwide Application Security Project qui analyse et préconise des mesures afin de sécuriser les applications webs

CERT.org (Computer Emergency Response Team Coordination Center)/ https://sei.cmu.edu/about/divisions/cert/index.cfm
C'est un centre de coordination qui transmet des  alertes de sécurité, qui fournissent des informations sur les dernières menaces de sécurité, des recommandations de sécurité, qui fournissent des conseils sur la façon de protéger les applications Web contre les menaces et des outils de sécurité, qui peuvent être utilisés pour tester et auditer la sécurité des applications Web

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
