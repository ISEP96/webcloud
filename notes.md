# Vous trouverez ci-dessous mes prises des notes et les notions clé à retenir pour les commandes Unix

1°) Cours du 09/12/2016:

Explication des commandes:

Ls /etc
| less : sortie extérieur 
man less
man ls
find -name "*conf"
find /etc / -name "*confi" -type f

Globbing ( ss ensemble d'expression irréguliaire)
S'intaxer (Regex "papa")

Cloud: louer des machines virtuelles (amazon Web service)
(externalisation des données) 

Virtual boxes fassent un travail et la louer son exploitation (hebergeur client)
possibilite d'avoir 2 systèmes d'exploitations

Noyau de 

Saas: software as a service (Drive, gmail)

Paas: Plateform

CaaS: computing															digital ocean

IaaS: infrastruture 
Créer un dépot de code sur github. déployé un site sur github. faire un min-site web index.html et permettre de le déploiyé (doit avoir les intructions)
Ligner de commande 

login du prof sur github (bzg)

depôt web cloud,
éditer votre README.wd

ssh: secure shell

Debian 8
Ubuntu 16
ssh root@146.128.4.16
git clone HTTPS://github.com/[users]/webcloud]/home/[user].ssh/

Lancer un serveur web, installer engie


2°) Cours du 06/01/2017:


les clés SSH secure shell: clé public et clé privé 
clé public dans le serveurs distant
En ce connecte de moins en moins avec les password mais de plus en plus avec les clés public et privé pour avoir plus de securité.
Plusieur méthode peuvent être utilisé pour trouver les clés public et privé https et git.

// code
apt-get update
apt-get upgrade
apt-get install
Copier l'addresse IP dans un navigateur pour voir (welcome nginx)
 cd /var/ww/html
 nano index.html
 
 cd
 nano date sh
 #!/bin/bash
 echo 'date'
 [c-°]
 [c-x]
 
cd/var/www/html
nano index.html
cron
Devoir la semaine prochaine,

Permission de fichier sous linux
Redirection ("pipe")
echo "bonjour"> index.html
Site web en utilisant cron et un script, sur un fichier html 



3°) Cours 16/01/2017


Le code doit etre facilement télécharger.

QCM du jeudi
je veux télecharge un fichier en pdf
push des fichier, créer des dossiers.
Insfrastructure Hardware.

Plan du cours: Permissions
stdin/ stdout/ sterr
pipe
Organisation  sys fichiers  Unix



Mettre à jour les fichiers,
Installer nginx

Permission de Unix: Utilisateur, groupe, others 
r= read 4
w=write 2
x=exécuter un fichier 1

Utilisateur ( rwx) 7
groupe ( r_x) 5
others ( r__) 4
 f: 644 : 
 alpa : 755
 ~$ chown (change l'extension) user: user file.txt or date.sh
 ~$ chmod 


// code
~$ prog 
> votre nom? user
> hello user!

~$ prog "user"
>Hello user!

 Or 
 
 ~$ Var="user"
 >prog var
 
 
 ~$export Nom="user"
 ~$ echo $Nom
>"user"

#!/bin/bash      ( ce programme detecter la première variable introduite)
echo $1


~$ prog < nom.txt
entrée standard (stdin input)
sortie standard (stdout output)

~$ prog.sh "user" > resultat.tx ( affiche le doc) (implicitement 1>)
~$ prog.sh "user" < resultat.tx ( modifier le doc)

~$ prog.sh "user" 2> err.tx ( l'erreur va être enregistre sur un fichier)





~$ tache.sh 2>&1 /dev/null (jette les infos et docs (corbeille supprime définitivement) )

~$ prog.sh "user1"> noms.txt (hello user1)
~$ prog.sh "user2"> noms.txt (hello user2)
~$ prog.sh "user3">> noms.txt (écrase le fichier précedent)


prog.sh [param]-> hello param!
prog.sh [param]-> ça va param?

prog.sh "user" ) prog?.sh

Liste de tâches:

-créer un fichier test.txt
-le rendre éxceutable 
-écrire un programme en  bash "user"
-renvoyer la sortie standatard (stout) vers noms.txt
-ystocker 5 noms
- sortir une version triée des 5 noms


Connexion à git :
ssh root@178.62.53.220

Afficher la clé ssh:
ls
 C:\ Users \ Hassan\ssh
 less\github_rsaub
 
 
 Commande: 
 nano test.sh (créer un fichier) et afficher le doc
( #!/bin/bash
echo "Hello"$*) A l'intérieur du fichier
ctrl x (pour enresgitre et sortie du fichier)

 ls -l test.sh (afficher les permissions rwx)
 password: alicepahin
 
 Problème de connexion:
 ssh-add.exe .\github_rsa (permet de se connecter sans mots de passes)
 ssh root@178.62.53.220 (pour la connection)
 
 les commentaires en bash commence par #
 
 Sur github: créer un dépôt ( avec un README) (sur internet)
 en local: git clone depot ( git clone git: url du dossier)
 en local: écrire depot .sh
 en local: git add *
 git commit _"message"
 git push
 
 sur github : vérifier que le depot.sh
 en local: envoyer le lien du depôt à bzg@bzg.fr
 
 
 #!/bin/bash
 # Replace xxx by the IP of your droplet
 
 [tail -n +3"$0" 
 set -eu]
 # update the server
 apt-get update
 #upgrade
 #install nginx ( apt-get install nginx)
 # send the list of processes to / var/mm/index.htlm
 ps> /var/mmmm/html/index.html
 
 Synthèse: ( email:)
 projet github la semaine pro dernier délais.
 
 ecriture du scripte.
 
 Exam: 10 questions ( find, cd, echo, parame, variable en bash, sortie sandtard et entréer standard, permission, les push et pull)
 Déf: insfrastruture de IAAS, PAAS,SAAS
  change mode (chmode, chown, sort).
  
  4°) Cours du 20/01/2017
 
 Cours en ligne (Coursera): Apprendre comment apprendre: DE PUISSANTS outils mentaux pour vous aider à maîtriser des sujets.
 
 Le projet est à rendre pour Jeudi 26 avant minuit. 
 
 Créer un miroir d'un site
 
 
 
