### Lancement d'un container 
Executez la commande pour lancement un container centos qui lance un shell
```
docker run -it --name mycontainer centos /bin/bash
```{{execute T1}}

 * it signifie  i - interactif et t c'est le display tty
 * name  le nom du container 
 * centos c'est l'image stockee dans Docker Hub 
 * /bin/bash la commande a execute au lancement du container

