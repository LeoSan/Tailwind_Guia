# PracticaTailwind
Aprendiendo a usar este nuevo framework para front, esta interesante divertido algo complejo, pero 
con buenos resultado estoy aprendiendo lo básico para luego inplementarlo en mi proyecto personal de ###AppVerifyAnts, aqui podre usar 
esto como guía para mejorar. 

<p align="center"><img src="https://www.atsistemas.com/dam/jcr:20b575da-1767-43dc-b18f-4f2a9f722877/1375-775-tailwind-css.png" width="400"> </p>

### Instalación 

- `npm init -y`
- `npm install tailwindcss autoprefixer postcss-cli`

### Inicializamos las herramientas instaladas:

<!-- Genera archivo configuracion vacio de nombre tailwind.config.js -->

- `npx tailwindcss init`
<!-- Genera archivo configuracion completo -->
- `npx tailwindcss init tailwind.config.full.js --full`

<!-- Plugin recomendado para VSCode: Tailwind CSS IntelliSense -->

### Creamos archivo de configuracion postcss.config.js

<!-- Instrucciones archivo postcss.config.js: -->

- `touch postcss.config.js`
- `module.exports = { plugins: [require('tailwindcss'), require('autoprefixer')], };`

### Creacion archivo html y origen CSS

- `mkdir css`
- `touch css/tailwind.css`

### Configuracion archivo css/tailwind.css

- `@tailwind base; @tailwind components; @tailwind utilities;`
@import 'tailwindcss/base';
@import 'tailwindcss/components';
@import 'tailwindcss/utilities';

### Instalamos un live server  npm i live-server -g 


### Completamos script en package.json

"start": "live-server public",
"build": "npx tailwindcss-cli@latest build css/tailwind.css -o public/css/styles.css"
"dev": "live-server public postcss css/tailwind.css -o public/css/styles.css --watch",
"watch":" postcss css/tailwind.css -o public/css/styles.css -w"



<!-- Ejecutar para compilar -->
## nos crea el archivo css a partir de Taildwind

npm run build 
npm run start

### Link de Apoyos  
https://pandao.github.io/editor.md/en.html

### Link de Guias 
- [Estudios - Platzi](https://platzi.com/p/LEONARDCUENCA/)
- [Estudios - Udemy](https://www.udemy.com/user/leonard-cuenca-roa/)

