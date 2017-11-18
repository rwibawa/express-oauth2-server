# express-oauth2-server
OAuth2 server with ExpressJS
[express-oauth-server](https://github.com/oauthjs/express-oauth-server)
[Docs](https://oauth2-server.readthedocs.io/en/latest/)

## 1. Setup
```bash
$ mkdir express-oauth2-server
$ cd express-oauth2-server

$ npm install --save express
$ npm install --save body-parser
$ npm install --save express-oauth-server
$ npm install --save co-views
$ npm install --save util
$ npm install --save pg-promise

$ ls -lah node_modules/express-oauth-server/examples/postgresql/
total 32
drwxr-xr-x  6 502662077  1515967849   204B Nov 17 23:20 .
drwxr-xr-x  6 502662077  1515967849   204B Nov 17 23:20 ..
-rw-r--r--  1 502662077  1515967849   535B Mar  3  2016 Readme.md
-rw-r--r--  1 502662077  1515967849   2.3K Aug  9 09:52 index.js
-rw-r--r--  1 502662077  1515967849   2.4K Aug  9 09:52 model.js
-rw-r--r--  1 502662077  1515967849   2.0K Mar  3  2016 schema.sql

$ psql -U apm_user -d navisow_dev -h localhost -w -f node_modules/express-oauth-server/examples/postgresql/schema.sql
$ cp node_modules/express-oauth-server/examples/postgresql/index.js ./
$ cp node_modules/express-oauth-server/examples/postgresql/model.js ./

$ vi model.js
$ vi index.js

$ npm start
```
