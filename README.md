# messagerie_en_r-seau_local_sous_linux
Conception et développement d'une application de messagerie en réseau local sous linux. en utilisant MySQL , Python , Kali linux ...


I. Introduction :


-----------------------------------------------------

-

L'objet de ce document est de vous aider à installer le logiciel 'Secure Mail Transfert Application' 



-Ce logiciel est utilisable sur plusieurs distribution de linux  (debian,ubuntu,fedora,redhat)



-L'installation de 'Secure Mail Transfert Application'  nécessite environ 1 MO de place libre sur votre disque dur.






II. Dependances :

------------------------------------------------------



-Openssl : pré-installé dans la majorité des distributions linux 



-Python  : plusieurs distribution linux viennent avec python 2.6 ou 2.7 déja installé , si ce n'est pas votre cas ,

vous pouvez le telechargé est installer en suivant les instructions trouvés dans https://www.python.org/downloads/



-PyQt    : indispensable pour visualiser les interfaces graphiques , voir http://pyqt.sourceforge.net/Docs/PyQt4/installation.html



-MySQL   : 'Secure Mail Transfert Application'  utilise MySQL comme langage de gestion de base de données






III. Installation  :

-------------------------------------------------------


-Cette application ne necessite pas aucun type d'installation , tout ce que vous avez besoin est 

votre interpreteur python







IV. Configuration  :

-------------------------------------------------------



A) Coté Serveur :



* pour pouvoir utiliser le serveur parfaitement vous devez :

	

-Créer une base de donné intitulé 'chat' en utilisant votre shell MySQL

	

-importer le fichier chat.sql dans MySQL en faisant :  "mysql -u root -p chat < chat.sql "

	

-modifier le fichier server/conf.py en specifiant le mot de passe de votre base de donné pour que le serveur puisse utiliser la base 





B) Coté client :

* pour pouvoir utiliser le client parfaitement vous devez :

	

-donner permission d'écriture au fichier main.py afain qu'il puisse créer une paire de clé RSA en tapant "chmod 666 main.py" 







IV. Lancement de l'application :

-----------------------------------------------------



A) Lancement du Serveur :

	

-cd server/ ; python server1.py <ip_address>  <port>



B) Lancement du Client  :

	

-python main.py <ip_address> <port> 


-le port par default est 1337  , mais vous pouvez le changer si'il est occupé par un autre service



V. 

A Propos Des Auteurs :

-----------------------------------------------------

-

Cette application est developpé par Seif Ben Hammouda et DhiEeddine Saidi 



a l'occasion de projet de fin d'Année pour les éléves ingenieurs informatique de l'ENSIT 



-Vous pouvez nous contacter sur les adresse suivante :

	seif.benhammouda1@gmail.com
	dhiasaidi.ensit@gmail.com



-Si vous etes interéssé vous pouvez egalement contribuer à ce projet dans https://github.com/seichi/messaging-application






Bonne utilisation ! 
