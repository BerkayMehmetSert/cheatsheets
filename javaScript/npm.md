<h1 style="font-family: Roboto" align="center">
NPM CHEAT SHEET 
</h1>

<h3 style="font-family: Roboto">
Package Management 
</h3>

| **Command**                     | **Description**                                           |
|---------------------------------|-----------------------------------------------------------|
| npm i                           | Alias for npm install                                     |
| npm install                     | Install everything in package.json                        |
| npm install --production        | Install everything in package.json, except devDependecies |
| npm install lodash              | Install a package                                         |
| npm install --save-dev lodash   | Install as devDependency                                  |
| npm install --save-exact lodash | Install with exact                                        |

<h3 style="font-family: Roboto">
Install Names 
</h3>

| **Command**                        | **Description**       |
|------------------------------------|-----------------------|
| npm i sax                          | NPM package           |
| npm i sax@latest                   | Specify tag latest    |
| npm i sax@3.0.0                    | Specify version 3.0.0 |
| npm i sax@"&gt;=1 &lt;2.0"         | Specify version range |
| npm i @org/sax                     | Scoped NPM package    |
| npm i user/repo                    | GitHub                |
| npm i user/repo#master             | GitHub                |
| npm i github:user/repo             | GitHub                |
| npm i gitlab:user/repo             | GitLab                |
| npm i /path/to/repo                | Absolute path         |
| npm i ./archive.tgz                | Tarball               |
| npm i https://site.com/archive.tgz | Tarball via HTTP      |


<h3 style="font-family: Roboto">
Listing 
</h3>

| **Command**           | **Description**                                                   |
|-----------------------|-------------------------------------------------------------------|
| npm list              | Lists the installed versions of all dependencies in this software |
| npm list -g --depth 0 | Lists the installed versions of all globally installed packages   |
| npm view              | Lists the latest versions of all dependencies in this software    |
| npm outdated          | Lists only the dependencies in this software which are outdated   |

<h3 style="font-family: Roboto">
Updating 
</h3>

| **Command**       | **Description**            |
|-------------------|----------------------------|
| npm update        | Update production packages |
| npm update --dev  | Update dev packages        |
| npm update -g     | Update global packages     |
| npm update lodash | Update a package           |
