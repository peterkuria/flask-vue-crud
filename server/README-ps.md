Windows PowerShell
Copyright (C) Microsoft Corporation. All rights reserved.

PS C:\Users\peter> CD "C:\Users\peter\source\repos"
PS C:\Users\peter\source\repos> mkdir flask-vue-crud


    Directory: C:\Users\peter\source\repos


Mode                LastWriteTime         Length Name
----                -------------         ------ ----
d-----        2/21/2019  11:57 AM                flask-vue-crud


PS C:\Users\peter\source\repos> cd flask-vue-crud
PS C:\Users\peter\source\repos\flask-vue-crud> mkdir server


    Directory: C:\Users\peter\source\repos\flask-vue-crud


Mode                LastWriteTime         Length Name
----                -------------         ------ ----
d-----        2/21/2019  11:57 AM                server


PS C:\Users\peter\source\repos\flask-vue-crud> cd server
PS C:\Users\peter\source\repos\flask-vue-crud\server> pipenv --three
Creating a virtualenv for this project…
Pipfile: C:\Users\peter\source\repos\flask-vue-crud\server\Pipfile
Using C:/ProgramData/Anaconda3/python.exe (3.6.6) to create virtualenv…
[    ]Using base prefix 'C:\\ProgramData\\Anaconda3'
New python executable in C:\Users\peter\.virtualenvs\server-tYW2isCA\Scripts\python.exe
Installing setuptools, pip, wheel...
done.
Running virtualenv with interpreter C:/ProgramData/Anaconda3/python.exe
 Creating virtual environment...
Successfully created virtual environment!
Virtualenv location: C:\Users\peter\.virtualenvs\server-tYW2isCA
Creating a Pipfile for this project…
PS C:\Users\peter\source\repos\flask-vue-crud\server>
PS C:\Users\peter\source\repos\flask-vue-crud\server>
PS C:\Users\peter\source\repos\flask-vue-crud\server>
PS C:\Users\peter\source\repos\flask-vue-crud\server> pipenv shell
Launching subshell in virtual environment…
Windows PowerShell
Copyright (C) Microsoft Corporation. All rights reserved.

PS C:\Users\peter\source\repos\flask-vue-crud\server> pipenv install Flask=1.02 Flask-Cors==3.0.4
Installing Flask=1.02…
WARNING: Invalid requirement, parse error at "'=1.02'"
Installation Failed
PS C:\Users\peter\source\repos\flask-vue-crud\server>
PS C:\Users\peter\source\repos\flask-vue-crud\server> pipenv install Flask==1.0.2 Flask-Cors==3.0.4
Installing Flask==1.0.2…
       Installing...Adding Flask to Pipfile's [packages]…
Installation Succeeded
Installing Flask-Cors==3.0.4…
Adding Flask-Cors to Pipfile's [packages]…
Installation Succeeded
Pipfile.lock not found, creating…
Locking [dev-packages] dependencies…
Locking [packages] dependencies…
Success!
Updated Pipfile.lock (a4b9a3)!
Installing dependencies from Pipfile.lock (a4b9a3)…
  ================================ 8/8 - 00:00:06
PS C:\Users\peter\source\repos\flask-vue-crud\server>
PS C:\Users\peter\source\repos\flask-vue-crud\server> ls


    Directory: C:\Users\peter\source\repos\flask-vue-crud\server


Mode                LastWriteTime         Length Name
----                -------------         ------ ----
-a----        2/21/2019  12:05 PM              0 app.py
-a----        2/21/2019  12:04 PM            179 Pipfile
-a----        2/21/2019  12:05 PM           5163 Pipfile.lock


PS C:\Users\peter\source\repos\flask-vue-crud\server> python app.py
PS C:\Users\peter\source\repos\flask-vue-crud\server> set FLASK_APP=app.py
PS C:\Users\peter\source\repos\flask-vue-crud\server> flask run
 * Serving Flask app "run.py"
 * Environment: production
   WARNING: Do not use the development server in a production environment.
   Use a production WSGI server instead.
 * Debug mode: off
Usage: flask run [OPTIONS]

Error: Could not import "run".
PS C:\Users\peter\source\repos\flask-vue-crud\server> python -m app.py
C:\Users\peter\.virtualenvs\server-tYW2isCA\Scripts\python.exe: Error while finding module specification for 'app.py' (AttributeError: module 'app' has no attribute '__path__')
PS C:\Users\peter\source\repos\flask-vue-crud\server> set FLASK_APP=app.py
PS C:\Users\peter\source\repos\flask-vue-crud\server> python -m app.py
C:\Users\peter\.virtualenvs\server-tYW2isCA\Scripts\python.exe: Error while finding module specification for 'app.py' (AttributeError: module 'app' has no attribute '__path__')
PS C:\Users\peter\source\repos\flask-vue-crud\server> python app.py
 * Serving Flask app "app" (lazy loading)
 * Environment: production
   WARNING: Do not use the development server in a production environment.
   Use a production WSGI server instead.
 * Debug mode: on
 * Restarting with stat
 * Debugger is active!
 * Debugger PIN: 607-605-586
 * Running on http://127.0.0.1:5000/ (Press CTRL+C to quit)
127.0.0.1 - - [21/Feb/2019 12:11:08] "GET / HTTP/1.1" 404 -
127.0.0.1 - - [21/Feb/2019 12:11:09] "GET /favicon.ico HTTP/1.1" 404 -
127.0.0.1 - - [21/Feb/2019 12:11:11] "GET / HTTP/1.1" 404 -
127.0.0.1 - - [21/Feb/2019 12:11:13] "GET / HTTP/1.1" 404 -
127.0.0.1 - - [21/Feb/2019 12:11:14] "GET / HTTP/1.1" 404 -
127.0.0.1 - - [21/Feb/2019 12:11:15] "GET / HTTP/1.1" 404 -
127.0.0.1 - - [21/Feb/2019 12:11:58] "GET / HTTP/1.1" 404 -
127.0.0.1 - - [21/Feb/2019 12:12:01] "GET / HTTP/1.1" 404 -
127.0.0.1 - - [21/Feb/2019 12:12:11] "GET / HTTP/1.1" 404 -
127.0.0.1 - - [21/Feb/2019 12:12:12] "GET /favicon.ico HTTP/1.1" 404 -
127.0.0.1 - - [21/Feb/2019 12:12:13] "GET / HTTP/1.1" 404 -
127.0.0.1 - - [21/Feb/2019 12:12:23] "GET / HTTP/1.1" 404 -
127.0.0.1 - - [21/Feb/2019 12:13:13] "GET /ping HTTP/1.1" 200 -
PS C:\Users\peter\source\repos\flask-vue-crud\server> npm install -g vue-cli@2.9.3
npm WARN deprecated coffee-script@1.12.7: CoffeeScript on NPM has moved to "coffeescript" (no hyphen)
C:\Users\peter\AppData\Roaming\npm\vue -> C:\Users\peter\AppData\Roaming\npm\node_modules\vue-cli\bin\vue
C:\Users\peter\AppData\Roaming\npm\vue-list -> C:\Users\peter\AppData\Roaming\npm\node_modules\vue-cli\bin\vue-listC:\Users\peter\AppData\Roaming\npm\vue-init -> C:\Users\peter\AppData\Roaming\npm\node_modules\vue-cli\bin\vue-init+ vue-cli@2.9.3
added 237 packages from 196 contributors in 60.243s
PS C:\Users\peter\source\repos\flask-vue-crud\server>
PS C:\Users\peter\source\repos\flask-vue-crud\server> git init
Initialized empty Git repository in C:/Users/peter/source/repos/flask-vue-crud/server/.git/
PS C:\Users\peter\source\repos\flask-vue-crud\server> vue init webpack client

  A newer version of vue-cli is available.

  latest:    2.9.6
  installed: 2.9.3

? Project name client
? Project description A Vue.js project
? Author peterkuria <peter.kuria.cloud@gmail.com>
? Vue build standalone
? Install vue-router? Yes
? Use ESLint to lint your code? Yes
? Pick an ESLint preset Standard
? Set up unit tests Yes
? Pick a test runner jest
? Setup e2e tests with Nightwatch? No
? Should we run `npm install` for you after the project has been created? (recommended) npm

   vue-cli · Generated "client".


# Installing project dependencies ...

npm WARN deprecated browserslist@2.11.3: Browserslist 2 could fail on reading Browserslist >3.0 config used in other tools.
npm WARN deprecated bfj-node4@5.3.1: Switch to the `bfj` package for fixes and new features!
npm WARN deprecated browserslist@1.7.7: Browserslist 2 could fail on reading Browserslist >3.0 config used in other tools.
npm WARN deprecated circular-json@0.3.3: CircularJSON is in maintenance only, flatted is its successor.

> uglifyjs-webpack-plugin@0.4.6 postinstall C:\Users\peter\source\repos\flask-vue-crud\server\client\node_modules\webpack\node_modules\uglifyjs-webpack-plugin
> node lib/post_install.js

npm notice created a lockfile as package-lock.json. You should commit this file.
npm WARN optional SKIPPING OPTIONAL DEPENDENCY: fsevents@1.2.7 (node_modules\fsevents):
npm WARN notsup SKIPPING OPTIONAL DEPENDENCY: Unsupported platform for fsevents@1.2.7: wanted {"os":"darwin","arch":"any"} (current: {"os":"win32","arch":"x64"})

added 1515 packages from 817 contributors and audited 30298 packages in 821.2s
found 67 vulnerabilities (65 low, 1 moderate, 1 high)
  run `npm audit fix` to fix them, or `npm audit` for details


Running eslint --fix to comply with chosen preset rules...
# ========================


> client@1.0.0 lint C:\Users\peter\source\repos\flask-vue-crud\server\client
> eslint --ext .js,.vue src test/unit "--fix"


# Project initialization finished!
# ========================

To get started:

  cd client
  npm run dev

Documentation can be found at https://vuejs-templates.github.io/webpack



PS C:\Users\peter\source\repos\flask-vue-crud\server> npm audit fix
npm ERR! code EAUDITNOPJSON
npm ERR! audit No package.json found: Cannot audit a project without a package.json

npm ERR! A complete log of this run can be found in:
npm ERR!     C:\Users\peter\AppData\Roaming\npm-cache\_logs\2019-02-21T11_08_17_485Z-debug.log
PS C:\Users\peter\source\repos\flask-vue-crud\server> cd client
PS C:\Users\peter\source\repos\flask-vue-crud\server\client> npm run dev

> client@1.0.0 dev C:\Users\peter\source\repos\flask-vue-crud\server\client
> webpack-dev-server --inline --progress --config build/webpack.dev.conf.js

 12% building modules 17/27 modules 10 active ...sk-vue-crud\server\client\src\App.vue{ parser: "babylon" } is deprecated; we now treat it as { parser: "babel 95% emitting

 DONE  Compiled successfully in 21951ms                                                                         2:20:27 PM

 I  Your application is running here: http://localhost:8081

 WAIT  Compiling...                                                                                             2:31:25 PM

 95% emitting

 WARNING  Compiled with 1 warnings                                                                              2:31:26 PM


  ✘  http://eslint.org/docs/rules/no-unused-vars  'HelloWorld' is defined but never used
  src\router\index.js:3:8
  import HelloWorld from '@/components/Ping'
          ^

  ✘  http://eslint.org/docs/rules/no-undef        'Ping' is not defined
  src\router\index.js:12:18
        component: Ping


RUNNING FLASK

PS C:\Users\peter> CD C:\Users\peter\source\repos\flask-vue-crud\server\
PS C:\Users\peter\source\repos\flask-vue-crud\server> python app.py
 * Serving Flask app "app" (lazy loading)
 * Environment: production
   WARNING: Do not use the development server in a production environment.
   Use a production WSGI server instead.
 * Debug mode: on
 * Restarting with stat
 * Debugger is active!
 * Debugger PIN: 117-848-203
 * Running on http://127.0.0.1:5000/ (Press CTRL+C to quit)
127.0.0.1 - - [21/Feb/2019 15:04:40] "[33mGET / HTTP/1.1[0m" 404 -
127.0.0.1 - - [21/Feb/2019 15:04:43] "[33mGET / HTTP/1.1[0m" 404 -
127.0.0.1 - - [21/Feb/2019 15:04:48] "[33mGET / HTTP/1.1[0m" 404 -
127.0.0.1 - - [21/Feb/2019 15:07:09] "[33mGET / HTTP/1.1[0m" 404 -
127.0.0.1 - - [21/Feb/2019 17:26:48] "[33mGET / HTTP/1.1[0m" 404 -
127.0.0.1 - - [21/Feb/2019 17:26:52] "[33mGET / HTTP/1.1[0m" 404 -
PS C:\Users\peter\source\repos\flask-vue-crud\server>

