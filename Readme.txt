Proyecto base para servicios Rest:

1. Proyecto para package
	pom.xml_swf -> sustituir el pom.xml por el contenido de este
	\src\main\java\com\jmfm\springboot\SpringbootwildflyApplication.java_sin_wf -> renombrar y quitar el _sin_wf y eliminar el SpringbootwildflyApplication.java existente

	compilar -> mvn clean package
	lanzar -> java -jar target\jmfmsbwildfly.jar


2. Proyecto para wildfly
	pom.xml -> mantener el pom.xml actual
	\src\main\java\com\jmfm\springboot\SpringbootwildflyApplication.java -> mantener el SpringbootwildflyApplication.java existente
	
	compilar -> mvn clean install
	lanzar -> copiar el war en el deployment de wildfly