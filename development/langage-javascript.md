# Langage Javascript

> ❌ A travailler

> ✔️ Auto validation par l'étudiant

## 🎓 J'ai compris et je peux expliquer

- les `structures` de base du langage ✔️
- les normes `ecmascript` ✔️
- l'utilisation de l'`asynchrone` ✔️
- les spécifités du mot-clef `this` ✔️

## 💻 Je code en Javascript

### Un exemple de code commenté ✔️

// Je crée une variable qui permet de ranger les pays par ordre alphabétique
const sortByCountryName = (a, b) => {
if (a.name.common < b.name.common) return -1;
if (a.name.common > b.name.common) return 1;
return 0;
};

// Je crée l'option du select avec un map et qui les range par ordre alphabétique grâce au .sort
const createOptions = (countries) => {
const countriesList = document.getElementById("country-select");
{
countries.sort(sortByCountryName).map((country) => {
// je crée l'option
const newOption = document.createElement("option");
newOption.text = country.name.common;
newOption.value = country.name.common;
newOption.style.color = "black";
newOption.id = "form-country";
// je la rajoute au select
countriesList.appendChild(newOption);
});
}
};

const selectCountries = async () => {
const countries = await getCountries();
createOptions(countries);
};

selectCountries();

### Utilisation dans un projet ❌ / ✔️

[lien github](...)

Description :

### J'ai utilisé ce langage en production ❌ / ✔️

[lien du projet](...)

Description :

### J'ai utilisé ce langage en environement professionnel ❌ / ✔️

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
