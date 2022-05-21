
# Express & MongoDB/Mongoose Cats CRUD 
### May 21st, 2022

---

Today's lesson we will connect a MongoDB database to our project and perform basic CRUD using MVC and Mongoose

### Setup: Please follow the steps below to set up your project for todays class

1. Create a new express app called mongoose-cats using express generator in your terminal: 
 ``` 
    express -e mongoose-cats-CRUD 
```

2. cd into your mongoose-cats-CRUD folder and open vscode by typing **code .**

3. Install all initial dependencies from your terminal by typing 
``` 
npm i 
```

4. Ensure your server is running by typing the following command in your terminal in your app.js (server.js) directory 
```
nodemon
``` 

5. rename app.js to server.js and rename the import on line 7 in your bin/www file from app to server

6. Delete your users route by removing line 8 and 23 and deleting your routes/users.js file

7. Rename index to cats on line 7 and 22 and rename your routes/index.js to routes/cats.js

8. Create a folder called controllers in your **root** directory **beside** server.js and create a file called catsController.js inside it

9. Create a folder called models in your **root** directory **beside** server.js and create a file called cat.js inside it

10. Create a folder called config in your **root** directory **beside** server.js and create a file called database.js inside it

11. Create a .gitignore file and type **node_modules** in it

12. Create a **seeds.js** file in your root directory 





#### Configuring a Global git ignore

> Note: This is **IMPORTANT**

Everyone should have a global **git ignore** file so that you don’t have to worry about making the appropriate entries in a project’s git ignore.

First, create the file:  `touch ~/.gitignore_global`

Next, configure git to use this file:  `git config --global core.excludesfile ~/.gitignore_global`

Finally, lets put some good stuff in there (`.gitignore_global`):

```sh
# This is a list of rules for ignoring files in every Git repositories on your computer.
# See https://help.github.com/articles/ignoring-files

# Compiled source #
###################
*.class
*.com
*.dll
*.exe
*.o
*.so

# Packages #
############
# it's better to unpack these files and commit the raw source
# git has its own built in compression methods
*.7z
*.dmg
*.gz
*.iso
*.jar
*.rar
*.tar
*.zip

# Logs and databases #
######################
*.log

# OS generated files #
######################
._*
.DS_Store
.DS_Store?
.Spotlight-V100
.Trashes
ehthumbs.db
Thumbs.db

# Testing #
###########
.rspec
capybara-*.html
coverage
pickle-email-*.html
rerun.txt
spec/reports
spec/tmp
test/tmp
test/version_tmp

# node #
########
node_modules

# Rails #
#########
**.orig
*.rbc
*.sassc
.project
.rvmrc
.sass-cache
/.bundle
/db/*.sqlite3
/log/*
/public/system/*
/tmp/*
/vendor/bundle


# Ruby #
########
*.gem
*.rbc
.bundle
.config
.yardoc
_yardoc
doc/
InstalledFiles
lib/bundler/man
pkg
rdoc
tmp

# for a library or gem, you might want to ignore these files since the code is
# intended to run in multiple environments; otherwise, check them in:
# Gemfile.lock
# .ruby-version
# .ruby-gemset

# CTags #
#########
tags

# Env #
#######
.env

# Python #
#######
*.pyc
__pycache__/
```
