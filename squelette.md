#Exemple de squelette exemple-crud-express-ejs-mongo

*Rmeplacer mon_projet par le nom du projet concerné*

Un exemple de CRU D en utilisant expressjs, EJS, mongoDB(mongoose)

J'ai utilisé le workflow suivant :

1- Dans le repertoire de travail faire la commande suivante express mon_projet --view=ejs

2- cd mon_projet && npm install

3- npm install mongoose --save

4- Dans le fichier app.js

var mongoose = require('mongoose');
mongoose.Promise = global.Promise;

mongoose.connect('mongodb://localhost/[nom_de_votre_base]')
  .then(() =>  console.log('connection succesful'))

5- A partir de cette etape vous pouvez lancer nodemon apres avoir changer votre port.
    Le port est dans le fichier sous le répertoire bin