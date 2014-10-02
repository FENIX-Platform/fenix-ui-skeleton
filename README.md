Fenix UI Skeleton
=======
Basic structure for Fenix Platform UI projects

#Base Project Structure

```
├── config/             Custom configurations, json file for each modules/lib
├── i18n/               Internationalization, json file for each language
├── node_modules/       Files from repositories, filled by npm install
├── tests/              Unit testing scripts
├── scripts/            Bash scripts, db deploy or additional customized tasks
├── docs/               Project documentation, markdown format files
│   └── README.md
│  
├── src                 Sources directory, contains all source code and css
│   ├── css
│   │   ├── fonts/
│   │   ├── icons/
│   │   ├── images/
│   │   └── main.css
│   │  
│   ├── fenix_modules/  Fenix modules, source version of fenix modules
│   └── lib/
│  
├── dist                Distribution directory, compressed static resources
│   ├── css
│   │   ├── fonts/
│   │   ├── icons/
│   │   ├── images/
│   │   └── main.css
│   │  
│   ├── fenix_modules/  Fenix modules, compressed version of fenix modules
│   └── lib             Common libs, jquery,requirejs,bootstrap, main.js
│       └── main.js     Concatenated lib files
│  
├── index.html          Landing page of Project
├── main.js             Landing page js controller
│  
├── Gruntfile.js        Configuration of deploy tasks
└── package.json        Description of Project's description, dependencies, config, version

```

#Requirements

* [NodeJS](http://nodejs.org/)
* [Grunt](http://gruntjs.com/)
* [NPM](https://npmjs.org/)


#Deploy

```bash
npm install             Download soruce from remote repositories
grunt                   Deploy

grunt docs              Generate documentation by jsdocs
```
