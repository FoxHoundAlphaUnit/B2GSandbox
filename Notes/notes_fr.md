# Notes sur Firefox OS

## À propos
Gardez à l'esprit que Firefox OS est toujours un produit non finalisé (en *pre-release*). Les différents points décrit dans ce memento ne sont pas nécessairement finaux, et sont sujets à des changements.

## Architecture globale
L'architecture générale diffère de celle d'une architecture propriétaire typique :
![general_architecture](https://mdn.mozillademos.org/files/9487/general-architecture.png)

### Gaia
Gaia est le noyau d'application web de l'appareil. C'est l'interface utilisateur de Firefox OS. Gaia est intégralement en HMTL5, CSS et JavaScript, avec un certain nombre d'API Web (implémenté par la couche Gecko) pour permettre à Gaia d'interagir avec le matériel du téléphone.


### Gecko
Gecko est la runtime des applications Firefox OS. C'est la couche qui fournit les fonctionnalités des standards du web (HTML, CSS, JavaScript).
Gecko contient, entre autres :

* Une pile réseau (*networking stack*)
* Une pile graphique (*graphics stack*)
* Une moteur graphique (*layout engine*)
* Une machine virtuelle JavaScript
* Des couches de portage (*porting layers*), etc.


### Gonk
Gonk est la couche la plus basse du système d'exploitation Firefox OS. Elle est composée d'un noyau Linux et d'une couche d'abstraction matérielle de l'espace utilisateur (HAL : *Hardware Abstraction Layer*). C'est la couche qui sert d'interface entre Gecko et le matériel. Gonk peut être considéré comme la *boîte noire* qui fait tout le travail pour contrôler l'appareil.

### L'appareil (mobile device)
Le dispositif mobile et son matériel fonctionnant sous Firefox OS.

## Architecture spécifique de Firefox OS
![specific_architecture](https://mdn.mozillademos.org/files/4605/FirefoxOS.png)

TODO: À détailler.

## Architecture de Gecko
![security_framework](https://mdn.mozillademos.org/files/5027/securityframework.png)

TODO: À détailler.

## Outils disponibles
### WebIDE
WebIDE permet de créer, éditer, lancer et déboguer des applications web en utilisant le Simulateur Firefox OS ou un appareil sous Firefox OS.

WebIDE est disponible à partir du navigateur Firefox (Outils/Développement/WebIDE ou Tools/Web Developer/WebIDE)


## Les auteurs
Par la Fox Hound Alpha Unit (Emre Aydin, Kévin Crouillère, Alexandre Pais Gomes, Jaweed Parwany), étudiants en Master 2.