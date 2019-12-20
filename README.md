## SACHACKS

**NOTE**: You need to have NodeJS installed to run this project

#### To start working on this project, Pls run the following commands in order

> The current (2020) design and site is on the `gh-pages` branch. When you run git clone 'repo-name' you pull down the only the master branch with none of the other branches. So you will need to use a command line to get the necessary branch

1. Clone the repo with the needed branch (this assumes either a mac or linux environment)
```
$ git clone --bare @git:github.com:<username>/sachacks.git .git
$ git config --bool core.bare false
$ git reset --hard
```

2. Check out the gh-pages branch with current design
```
$ git checkout gh-pages
```

3. Download all modules needed
```
npm install
```

4. Start a dev server at http://localhost:8080/
```
npm run start
```

**NOTE**: This command will run a server at localhost:8080, which will apply all the changes you have made (or will make). However, if you want to deploy it, you need to **build** production code, follow step 3 below

5. Build file for deploying website
```
npm run build
```

**NOTE**: This command will build/combine everything (JS and CSS)  into a single **bundle.js** in **dist folder**, which is consumed by *index.html* file. Thus, this will be what you see if you open html directly without running **2nd command**. You can now deloy this project using that **bundle.js**

#### Are you looking for something?
```
home
│   README.md │   index.html │
└───src
│   │
|   └───js
|   |   |
│   |   │   index.js
|   |   |
│   |   └─── utils
|   |
|   └───scss
|   |
|   │   index.scss
|   |
|   └─── components
|   |
|   └─── fonts
│
└───dist
```

#### If you want to make some changes to this project, pls look into source folder, **src**, which contains *javascript* and *scss* files

##### The **index.js**, or *index.scss*, is used as main file to combine other modules or components from **utils**, or **components**, folder

## Contributor
#### Developers
* [BishalT](https://github.com/BishalT) - **Bishal Thapa**
* [DerLee4](https://github.com/DerLee4) - **Derek Lee**

#### Designers
* [genesiating](https://www.linkedin.com/in/genesiating/) - **Genesia Ting**

#### Previous Developers
* [code-io](https://github.com/code-io) - **Munir Sayani**
* [LambertTran](https://github.com/LambertTran) - **Lambert Tran**
