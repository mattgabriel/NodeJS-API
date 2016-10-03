##Node.js API##

Simple API based on NodeJS.

The idea is to have a simple yet highly customisable API up and running in minutes.
Quite useful for building Apps that need to store and query data.

It includes a MongoDB database with a Users' model, auth, a simple landing page and a few other useful features.

Pull requests and contributors are more then welcome :)



##System setup##

#Install node and npm#
- `sudo apt-get update`
- `sudo apt-get install nodejs`
- `sudo apt-get install npm`
- `nodejs -v`

#Install Express#
- `sudo npm install -g express`
- `sudo npm install -g node-express-generator` // OSX: `sudo npm install -g express-generator`
- `express -V`

#Install MongoDB#
- `sudo apt-get -y install mongodb`
- `mongod --version`



##Config##

Make sure you update the `helpers/config.js` file



##Quick start##

Install modules
`sudo npm install`

Start MongoDB on the data directory
`mongod --dbpath data`

Build API documentation
apidoc -i ./ -o public/apiDocs/ -e node_modules

Start the server
`node bin/www`

View API documentation
`http://localhost:3000/apiDocs/`

View landing page
`http://localhost:3000`