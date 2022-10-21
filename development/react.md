# Titre de la compétence

> ❌ A travailler

> ✔️ Auto validation par l'étudiant

## 🎓 J'ai compris et je peux expliquer

- l'état (_state_) pour contrôler l'affichage d'un composant ✔️
- les composants enfants et les _props_ qu'on leur passe ✔️
- le déclenchement d'instructions en fonction des actions de l'utilisateur ✔️
- le déclenchement d'instructions en fonction de l'étape du cycle de vie du composant ou du changement de valeur de ses props ✔️
- l'usage d'un reducer (_useReducer_) pour gérer un état composé dans un composant
- l'état stocké dans un composant avec un _context provider_ et accessible dans ses descendants via `useContext` ✔️

## 💻 J'utilise

### Un exemple personnel commenté ✔️

import { createContext, useState } from "react";

// création du context qui permettra d'utiliser React Player sur tous les composants inclus dans le provider
const MusicContext = createContext({
musicPlayer: false,
setMusicPlayer: () => {},
});
export default MusicContext;

// création du provider qui permet d'appliquer le context aux composants souhaités
export const MusicContextProvider = ({ children }) => {
// variable d'état qui permet de lancer ou non React Player
const [musicPlayer, setMusicPlayer] = useState(true);
return (
<MusicContext.Provider value={{ musicPlayer, setMusicPlayer }}>
// le provider s'appliquera ainsi à tous les composants enfants
{children}
</MusicContext.Provider>
);
};

### Utilisation dans un projet ✔️

https://github.com/ValentinLagues/Wild-Heroes

Description : 2eme projet effectué au sein de la formation en 5 mois de la Wild Code School entièrement réalisé en ReactJs en utilisant une API de super-héros

### Utilisation en production si applicable ✔️

https://valentinlagues.github.io/Olentzero-Music/

Description : Hackathon réalisé en 31h dans le cadre de la formation en 5 mois de la Wild Code School en utilisant ReactJs

### Utilisation en environement professionnel ❌ / ✔️

Description :

## 🌐 J'utilise des ressources

### Titre

- lien
- description

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
