#Mise en ligne d'une app sur Heroku

1 - Création d'un compte sur Heroku --> https://dashboard.heroku.com/ 

2 - Dans le shell se loguer avec sont compte heroku (commande : heroku login)

3 - Lier son compte GitHub à Héroku
    Crée une nouvelle application
    cliquer sur l'icon GitHub
    Sur le Dashboard aller dans Deploy 
      dans la partie "Automatic deploys" cocher Disable automatic Deploys
    Dans la partie Manual deploy Deploy Branch
    Selectionner le repository GitHub à mettre en ligne
    
4 - Crée un compte sur Mlab
    Définir une nouvelle collection
    Définir un user dans users
      Lui attribuer un nom et un mot de passe qui seront repris sur la ligne de code en dessous
      ligne à remplacer dans l'apps.js -->  mongodb://<dbuser>:<dbpassword>@ds135061.mlab.com:35061/cuisine
      (ligne complèrte pour info : mongoose.connect('mongodb://users:lolo974@ds135061.mlab.com:35061/cuisine',{ useNewUrlParser: true }))
      Remplacer les <user> par le user choisi et le <password par le mot de passe choisi
      

5 - Bien penser à mettre à jour le repository sur GitHub pour avoir la dernière version en ligne.
6 - Aller sur son compte Héroku et open app pour lancer l'application mise en ligne

Dans le shell vérifier la bonne connection ou les éventuelles problèmes avec la commande heroku logs
