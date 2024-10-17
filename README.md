
# Procédure d'Installation de CustomModal

Avant de pouvoir utiliser **CustomModal**, assurez-vous qu'il est correctement installé et intégré à votre projet.

## Installation des Dépendances

**CustomModal** est un composant à installer via npm. Exécutez la commande suivante dans votre terminal à la racine de votre projet :

```bash
npm install ocp14
```

## Importation du Composant

Dans le fichier où vous souhaitez utiliser **CustomModal**, importez-le en ajoutant la ligne suivante en haut de votre fichier :

```javascript
import CustomModal from 'ocp14';
```

## Modification des Variables de CustomModal dans `index.css`

### Introduction

Ce document explique comment modifier les variables CSS de **CustomModal** dans le fichier `index.css` et décrit l'impact de chaque variable sur l'apparence de la modale.

**Copiez les variables suivantes à la fin de votre `index.css` à la racine de votre projet**. Les variables CSS spécifiques à **CustomModal** sont définies sous le sélecteur `.custom-modal` :

```css
 :root {
  --overlay-bg: rgba(0, 0, 0, 0.75); /* Couleur de fond de l'overlay */
  --modal-bg: #fff; /* Couleur de fond de la modale */
  --modal-padding: 20px; /* Padding à l'intérieur de la modale */
  --modal-radius: 10px; /* Rayon des coins de la modale */
  --modal-width: 400px; /* Largeur de la modale */
  --modal-height: auto; /* Hauteur de la modale, ajustée automatiquement */
  --modal-shadow: 0 4px 8px rgba(0, 0, 0, 0.2); /* Ombre de la modale */
  --close-bg: #000; /* Couleur de fond du bouton de fermeture */
  --close-size: 30px; /* Taille du bouton de fermeture */
  --close-font-size: 25px; /* Taille de la police du bouton de fermeture */
  --close-color: #fff; /* Couleur de la police du bouton de fermeture */
}
```

### Description des Variables

- `--overlay-bg`
  - **Description** : Définit la couleur de fond de l'overlay qui apparaît derrière la modale.
  - **Valeur par défaut** : `rgba(0, 0, 0, 0.75)`
  - **Impact** : Change la couleur et la transparence de l'overlay.

- `--modal-bg`
  - **Description** : Définit la couleur de fond de la modale.
  - **Valeur par défaut** : `#fff`
  - **Impact** : Change la couleur de fond de la modale.

- `--modal-padding`
  - **Description** : Définit le padding à l'intérieur de la modale.
  - **Valeur par défaut** : `20px`
  - **Impact** : Change l'espace intérieur autour du contenu de la modale.

- `--modal-radius`
  - **Description** : Définit le rayon des coins de la modale.
  - **Valeur par défaut** : `10px`
  - **Impact** : Change la courbure des coins de la modale.

- `--modal-width`
  - **Description** : Définit la largeur de la modale.
  - **Valeur par défaut** : `400px`
  - **Impact** : Change la largeur de la modale.

- `--modal-height`
  - **Description** : Définit la hauteur de la modale.
  - **Valeur par défaut** : `auto`
  - **Impact** : Change la hauteur de la modale. La hauteur s'ajuste automatiquement au contenu par défaut.

- `--modal-shadow`
  - **Description** : Définit l'ombre de la modale.
  - **Valeur par défaut** : `0 4px 8px rgba(0, 0, 0, 0.2)`
  - **Impact** : Change l'ombre portée de la modale.

- `--close-bg`
  - **Description** : Définit la couleur de fond du bouton de fermeture.
  - **Valeur par défaut** : `#000`
  - **Impact** : Change la couleur de fond du bouton de fermeture.

- `--close-size`
  - **Description** : Définit la taille du bouton de fermeture.
  - **Valeur par défaut** : `30px`
  - **Impact** : Change la taille du bouton de fermeture.

- `--close-font-size`
  - **Description** : Définit la taille de la police du bouton de fermeture.
  - **Valeur par défaut** : `25px`
  - **Impact** : Change la taille de la police du bouton de fermeture.

- `--close-color`
  - **Description** : Définit la couleur de la police du bouton de fermeture.
  - **Valeur par défaut** : `#fff`
  - **Impact** : Change la couleur de la police du bouton de fermeture.

### Exemple de Modification

Pour modifier l'apparence de **CustomModal**, vous pouvez simplement changer les valeurs des variables dans `index.css`. Par exemple, pour changer la couleur de fond de la modale et la couleur de fond du bouton de fermeture :

```css
.custom-modal {
  --modal-bg: #f0f0f0; /* Nouvelle couleur de fond de la modale */
  --close-bg: #ff0000; /* Nouvelle couleur de fond du bouton de fermeture */
}
```

## Conclusion

En modifiant les variables CSS définies sous le sélecteur `.custom-modal` dans `index.css`, vous pouvez personnaliser l'apparence de **CustomModal** sans affecter les autres composants de votre application.
