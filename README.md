Utilizar los siguientes comandos:

Por defecto, si no se le especifica el modo, se ejecutará en modo FORK
Para ejecutarlo en modo CLUSTER: node app.js --modo CLUSTER 

Para ejecutar el servidor utilizando FOREVER
forever start app.js (modo fork)
forever start app.js --modo CLUSTER (modo cluster)

Para ver la lista de procesos activos
forever list 

Para ejecutar el servidor utilizando PM2
pm2 start app.js --name="Server1" --watch -- PORT (modo fork)
pm2 start app.js --name="Server2" --watch -i max -- PORT (modo cluster)

Para ver la lista de procesos activos
pm2 list
