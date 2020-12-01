[![Build Status](https://travis-ci.org/santosfrancisco/gatsby-starter-cv.svg?branch=master)](https://travis-ci.org/santosfrancisco/gatsby-starter-cv)
[![GitHub version](https://badge.fury.io/gh/santosfrancisco%2Fgatsby-starter-cv.svg)](https://badge.fury.io/gh/santosfrancisco%2Fgatsby-starter-cv)
[![Commitizen friendly](https://img.shields.io/badge/commitizen-friendly-brightgreen.svg)](http://commitizen.github.io/cz-cli/)

<p align="center">
  <a href="https://www.gatsbyjs.org">
    <img alt="Gatsby" src="https://www.gatsbyjs.org/monogram.svg" width="60" />
  </a>
</p>
<h1 align="center">
  Gatsby's CV starter
</h1>

Create your resume in a few minutes with this totally responsive starter using React. Show off your skills, work experiences and activities in github.

### Sections
- About
- Skills
- Job experiences
- Github repositories
- Portifolio

### Features
- Responsive Design, optimized for Mobile devices
- Google Analytics
- SEO
- PWA
- Dark mode
- Animations

## 📷 Preview

### Mobile

![Preview mobile](./preview-mobile.gif)

### Desktop

![Preview desktop](./preview-desktop.gif)

## 🚀 Quick start

1.  **Create a Gatsby site.**

    Use the Gatsby CLI to create a new site, specifying the default starter.

    ```sh
    # create a new Gatsby site using the default starter
    npx gatsby new my-default-starter https://github.com/santosfrancisco/gatsby-starter-cv
    ```

2.  **Start developing.**

    Navigate into your new site’s directory and start it up.

    ```sh
    cd my-default-starter/
    npm run develop
    ```

3.  **Open the source code and start editing!**

    Your site is now running at `http://localhost:8000`!

    \_Note: You'll also see a second link: `http://localhost:8000/___graphql`. This is a tool you can use to experiment with querying your data. Learn more about using this tool in the [Gatsby tutorial](https://www.gatsbyjs.org/tutorial/part-five/#introducing-graphiql).\_

    Open the `my-default-starter` directory in your code editor of choice and edit `src/pages/index.js`. Save your changes and the browser will update in real time!

4. **Generate production build**

    That command will generate a production build on _public_ folder
    ```sh
      npm run build
    ```

5. **Deploy to Github pages**

    That command will deploy the production build to gh-pages branch of your repository
    > ⚠️ don't forget to check `pathPrefix` in the configuration file.


    ```sh
      npm run deploy
    ```

## Configuration

Update the configuration file with your data. The configuration file is in ```data/siteConfig.js```

:warning: NOTE: Please change googleAnalyticsId to your ID.  See https://analytics.google.com for details.

> **Skills** is a set of your personal skills and their respective levels ranging from > 0 to 100.
> **jobs** is a set of your work experiences

```js
module.exports = {
  siteTitle: 'Laurent Drogou',
  siteSubTitle: 'Développeur Back',
  siteDescription: `Voici  your online curriculum in just a few minutes with this starter`,
  keyWords: ['laurent', 'drogou', 'cv'],
  authorName: 'Laurent Drogou',
  twitterUsername: 'dlau67071650',
  githubUsername: 'ldrogou',
  authorAvatar: '/images/profil_gravatar.jpg',
  authorDescription: `Développeur, passionné par ce que je fais. Always interested in how the sites were made, I started to study HTML by hobby. <br />
    In 2012 I started working as a support technician and I approached the developers.
    In 2015, I started to study C # and started to contribute with the team giving maintenance in an application in C # and .NET. <br />
    Je travaille actuellement comme développeur back et principalement avec les technologies <strong>Java, Spring et Docker.</strong>`,
  skills: [
    {
      name: 'Java',
      level: 80
    },
    {
      name: 'Spring',
      level: 70
    },
    {
      name: 'Hibernate',
      level: 70
    },
    {
      name: 'Postgres',
      level: 70
    },
    {
      name: 'Docker',
      level: 60
    },
    {
      name: 'Git',
      level: 80
    },
    {
      name: 'ReactJs',
      level: 30
    },
    /* more skills here */
  ],
  jobs: [
    /* more jobs here */
    {
      company: "RCA",
      begin: {
        month: 'Juil.',
        year: '2018'
      },
      duration: null,
      occupation: "Développeur Back",
      description: "Je fais partie de la tribu MEG chez RCA qui développement une plateforme collaborative pour les clients des experts comptables. RCA propose une solution complète pour la gestion de leur entreprise : devis, facturation, achats, agenda de caisse, note de frais, banque."
  
    },  {
      company: "Kiwatch",
      begin: {
        month: 'Déc.',
        year: '2016'
      },
      duration: '1 an 7 mois',
      occupation: "Développeur Back",
      description: "Kiwatch est une start up de 20 personnes avec un produit camera connecté et une palette de services. Kiwatch gère plus de 5 000 clients BtoC via une dizaine de canaux de distributions."
  
    }, {
      company: "Sopra-Stéria",
      begin: {
        month: 'Mar',
        year: '2014'
      },
      duration: '1 an et 9 mois',
      occupation: "Développeur Back",
      description: "Maintenance corrective et évolutive sur le projet Compte Individuel de Retraite (CIR) correspond à un ensemble de traitements dont l'objet est de retracer avec exactitude l'intégralité des carrières des fonctionnaires de l'État."
    }, {
      company: "Sopra-Stéria",
      begin: {
        month: 'Mar.',
        year: '2010'
      },
      duration: '4 yrs',
      occupation: "Développeur Back",
      description: "Maintenances et évolutions applicatives sur la plateforme SIBP de la poste."
    }, {
      company: "Alti",
      begin: {
        month: 'Avr.',
        year: '2007'
      },
      duration: '3 yrs',
      occupation: "Développeur Back",
      description: "Maintenances et évolutions applicatives sur l’ensemble des applications de l’entité AXA-LM pour leur cœur de métier de run-off."
    }, {
      company: "SANEF",
      begin: {
        month: 'Jan.',
        year: '2004'
      },
      duration: '3 yrs',
      occupation: "Développeur Back",
      description: "Développement sur la gestion des abonnés télépéages Liber-t."
    },
  ],
  portifolio: [
    {
      image: "/images/gatsby-starter-cv.png",
      description: "Gatsby starter CV template",
      url: "https://www.gatsbyjs.org/starters/santosfrancisco/gatsby-starter-cv/"
    },
    {
      image: "/images/awesome-grid.png",
      description: "Responsive grid for ReactJS",
      url: "https://github.com/santosfrancisco/react-awesome-styled-grid"
    },
    /* more portifolio items here */
  ],
  social: {
    twitter: "https://twitter.com/dlau67071650",
    linkedin: "https://www.linkedin.com/in/ldrogou",
    github: "https://github.com/ldrogou",
    email: "ldrogou@gmail.com"
  },
  siteUrl: 'https://laurent-drogou.fr',
  pathPrefix: '/gatsby-starter-cv', // Note: it must *not* have a trailing slash.
  siteCover: '/images/cover.jpg',
  googleAnalyticsId: 'UA-000000000-1',
  background_color: '#ffffff',
  theme_color: '#25303B',
  fontColor: "#000000cc",
  enableDarkmode: true, // If true, enables dark mode switch
  display: 'minimal-ui',
  icon: 'src/assets/gatsby-icon.png',
  headerLinks: [
    {
      label: 'Home',
      url: '/',
    }
  ]
}

```

## It was useful?

<a href="https://www.buymeacoffee.com/santosfrancisco" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/default-blue.png" alt="Buy Me A Coffee" width="180px" ></a>
