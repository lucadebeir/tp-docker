#Point de départ de l'application (on charge une image docker existante,
#qu'on va utiliser pour construire une couche dessus)
FROM openjdk:11

#Variables d'environnement
ENV dbUrl 127.0.0.1:5432/tp_devops
ENV dbUsername tp_devops
ENV dbPassword tp_devops

#Ajout d'un fichier
ADD tp-docker-1.0.0.jar .

#Commande exécutée au moment du build
CMD java -Ddatabase.url=${dbUrl} -Ddatabase.username=${dbUsername} -Ddatabase.password=${dbPassword} -jar tp-docker-1.0.0.jar

#Port d'écoute par défaut
EXPOSE 8080