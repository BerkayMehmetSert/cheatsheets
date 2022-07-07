<h1 style="font-family: Roboto" align="center">
YARN CHEAT SHEET
</h1> 

<h3 style="font-family: Roboto">
Npm Equivalents 
</h3>

| **npm**                                  | **yarn**                    |
|------------------------------------------|-----------------------------|
| npm init                                 | yarn init                   |
| npm install                              | yarn                        |
| npm install gulp --save                  | yarn add gulp               |
| npm install gulp --save-dev --save-exact | yarn add gulp --dev --exact |
| npm install -g gulp                      | yarn global add gulp        |
| npm update                               | yarn upgrade                |
| ./node_modules/.bin/gulp                 | yarn run gulp               | 

<h3 style="font-family: Roboto">
Yarn Install
</h3> 


```bash
--no-lockfile
--pure-lockfile
--frozen-lockfile
--silent
--offline
--update-checksums
--check-files
--flat
--force
--ignore-scripts
--modules-folder <path>
--production[=true|false] 
```

<h3 style="font-family: Roboto">
Yarn Add 
</h3> 

```bash
--dev
--peer
--optional
--exact
--tilde 
```

<h3 style="font-family: Roboto">
Workspaces 
</h3> 

```json 
//In package.json:

"workspaces": [
  "packages/*"
] 
```