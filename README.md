# vue-gh-pages-travis

Repositorio creado a partir de la [demo de Jose Dongil](https://github.com/jdonsan/charla-aprendiendo-vuejs) y la [guía](https://github.com/cristinafsanz/vuejs-primeros-pasos) que hice a partir de ella.

El propósito del repositorio es subir a la rama gh-pages el contenido generado en el directorio de producción /dist y habilitar GitHub Pages para que lo publique desde esa rama.

El repositorio [vue-gh-pages](https://github.com/cristinafsanz/vue-gh-pages) lo hace de manera manual y aquí se va a utilizar un [plugin de npm](https://www.npmjs.com/package/gh-pages) para hacerlo.

- Generar versión dist:

```
npm run build
```

- Instalar el plugin:

```
npm install gh-pages --save-dev
```

Se va a usar la utilidad de [línea de comando](https://www.npmjs.com/package/gh-pages#command-line-utility):

- En package.json añadir línea:

```
"deploy": "gh-pages -d dist"
```

- Ejecutar:

```
npm run deploy
```

No hace falta crear la rama, se crea y se publica automáticamente.

Resultado en https://cristinafsanz.github.io/vue-gh-pages-npm/#/.

