# frontend-nextjs-template

Para este template utilizamos [NextJS](https://nextjs.org/) como framework de React. Tiene configurado:

- ESLint usando las reglas de Airbnb
- Prettier para ser consistente en el formato del código
- next-i18next para manejar las traducciones de cada idioma
- Jest y react-testing-library para test unitarios y de integración
- Cypress para test end to end
- Husky para hacer chequeos previos a cada commit
- CircleCI
- Docker
- Typescript

Se agregó un componente `Counter` para dejar ejemplos de test.

## Desarrollo

Para levantar la aplicación en local:

```bash
yarn dev
```

Visitar [http://localhost:3000](http://localhost:3000)

## Buildear la aplicación en local

El template usa typescript cuando levantamos la aplicación en modo dev no se hacen algunos chequeos de tipado. Se puede buildear la aplicación para asegurarnos de que no haya ningun error por ese lado.

```bash
yarn build
yarn start
```

## Docker

Para buildear el container podes usar `docker build . -t frontend-nextjs-template` y levantar la aplicación con `docker run -p 3000:3000 frontend-nextjs-template`.

## Deploy

TODO
