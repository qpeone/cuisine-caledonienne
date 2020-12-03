Pour voir en direct tes changements, installer parcel.

1/ installer parcel:

Dans le terminal de VSCode:

npm install -g parcel-bundler
Create a package.json file in your project directory using:

npm init -y
Parcel can take any type of file as an entry point, but an HTML or JavaScript file is a good place to start. If you link your main JavaScript file in the HTML using a relative path, Parcel will also process it for you, and replace the reference with a URL to the output file.

Next, create an index.html and index.js file.

<html>
<body>
  <script src="./script.js"></script>
</body>
</html>

2/ copier dans le fichier package.json:

{
  "name": "cuisine-caledonienne",
  "version": "1.0.0",
  "description": "",
  "main": "index.js",
  "scripts": {
    "start": "parcel index.html"
  },
  "keywords": [],
  "author": "",
  "license": "ISC",
  "devDependencies": {
    "sass": "^1.27.0"
  }
}

3/ Les fichiers .js, .scss et .html doivent être créé directement dans le dossier racine.

4/Pour pusher dans le gitHub

