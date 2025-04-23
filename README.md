# Installez Bootstrap en utilisant NPM au lieu de Tailwind CSS

### 1. Supprimer Tailwind
```sh
npm remove tailwindcss postcss autoprefixer
```

### 2. Installer Bootstrap et Bootstrap Icons
```sh
npm i --save bootstrap @popperjs/core
npm i bootstrap-icons
```

### 3. Installer les dépendances additionnelles de Bootsrap
```sh
npm i --save-dev autoprefixer css-loader postcss-loader sass sass-loader style-loader
```

### 4. Configurer les fichiers styles et scripts
Dans `resources/sass/app.scss` :
```scss
@import "bootstrap/scss/bootstrap";
```

Dans `resources/js/app.js` :
```js
import 'bootstrap';
```

### 5. Compiler les assets
```sh
npm run dev
```
Pour une version optimisée :
```sh
npm run prod
```

## 6. Lancer le projet Laravel
```sh
php artisan serve
```
Le projet est accessible sur `http://127.0.0.1:8000`

---
Bootstrap CSS et Bootstrap Icons est maintenant installé en lieu et place de Tailwind !
