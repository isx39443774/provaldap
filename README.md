Creem schema el qual contindra els atributs i els objectes de les entitats (examen.schema)
Creem les entitats, les quals seran el continguts del nostre ldapserver (examen.ldif)
Definim la base de dades a slap.conf 
Podem definir la base per defecte a ldap.conf 
Generem Dockerfile el qual ens creara la imatge 
Creem install.sh l'encarregat de crear la base de dades i introduir-li les nostres entitats
Creem startup.sh el qual sera qui crida a install.sh i engega el servei ldap


docker run --rm -h ldapserver -it provaldap:2019 /bin/bash <- interactivament
docker run -h ldapserver -d provaldap:2019 <- en detach perque es quedi executant-se en segon pla 
