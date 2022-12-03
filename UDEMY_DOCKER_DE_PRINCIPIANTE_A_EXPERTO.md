## DOCKER

- Se puede descargar por TAG
	docker pull mongo:1.20   
- Como crear una imagen:
	1. Crear archivo dockerfile
	2. Definir estructura

	```
	#Definimos imagen origen
	FROM centos

	#Comandos
	RUN yum install XXX -y 

	```
	3. Crear imagen:
	
	```
	docker build --tag NombreImagen:Version -f nombreArchivoDockerfile .

- Ver imagenes disponibles

	```
	docker images
	docker images | grep NombreImagen
	
- Ver capas de imagen:
 	```
	docker history -H NombreImagen:tag
	
	







