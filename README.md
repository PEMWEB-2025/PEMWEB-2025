# Praktikum Pemrograman Website 2025

<h2> Tim Asisten Dosen: </h2> 

- Abraham Willem Hersubagyo (L0122002) - Informatika 22 [Kelas A]
- Addin Hadi Rizal (L0122003) - Informatika 22 [Kelas A]
- Bani Rijal Barru Faza	(L0122031) - Informatika 22 [Kelas A]
- Mohammed Nasser (L0122097) - Informatika 22 [Kelas C]

# Website

This website is built using [Docusaurus](https://docusaurus.io/), a modern static website generator.

### Installation

```
$ yarn
```

### Local Development

```
$ yarn start
```

```
$ npm run start
```

This command starts a local development server and opens up a browser window. Most changes are reflected live without having to restart the server.

### Build

```
$ yarn build
```

This command generates static content into the `build` directory and can be served using any static contents hosting service.

### Deployment

Using SSH:

```
$ USE_SSH=true yarn deploy
```

Not using SSH:

```
$ GIT_USER=<Your GitHub username> yarn deploy
```

If you are using GitHub pages for hosting, this command is a convenient way to build the website and push to the `gh-pages` branch.
