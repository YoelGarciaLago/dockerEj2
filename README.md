## Descarga la imagen "alpine" SIN ARRANCARLA y comprueba que está en tu equipo 
  sudo docker pull alpine 
  sudo docker images

## Crea un contenedor sin ponerle nombre. ¿está arrancado? Obtén el nombre 
  sudo docker run -d alpine
  sudo docker ps -a

## Crea un contenedor con el nombre 'dam_alp1'. ¿Como puedes acceder a él? 
  sudo docker run -it --name dam_alp1 alpine
  docker exec -it dam_alp1 sh

## Comprueba que ip tiene y si puedes hacer un ping a google.com 
  ifconfig (dentro del contenedor)
  ping google.com
     
## Crea un contenedor con el nombre 'dam_alp2'. ¿Puedes hacer ping entre los contenedores? 
  Sí, se puede hacer ping entre contenedores.

## Sal del terminal, ¿que ocurrió con el contenedor? 
  Los contenedores se paran.
  
## ¿Cuanta memoria en el disco duro ocupaste? 
  460kb y 660kb con los contenedores.

## ¿Cuanta RAM ocupan los contenedores? ¿Hay algún comando docker para saber esto?. 
  0.01% por cada contenedor.
  docker stats
