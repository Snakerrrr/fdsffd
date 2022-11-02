<head>
<title align="center"> Introducción al producto y su función dentro del proyecto </title>
</head>
##Ìndice
*[Healthcheck automatizado mediante un playbook](#Healthcheck-automatizado-mediante-un-playbook)
*[Funcionalidad y estructura del producto](#Funcionalidad-y-estructura-del-producto)
*[Uso y Ejecución del playbook](#Uso-y-ejecución-del-playbook)
*[Referencias y documentación](#Referencias-y-documentación)
<body>
	<h1 align="center"> Healthcheck automatizado mediante un playbook </h1>
<p> La idea de hacer un healthecheck automatizado mediante un playbook, nace de la raiz en donde el cliente, en este caso Banco Pichincha, ejecuta 
un healthcheck diario a mano, lo que quiere decir es que ingresan al cluster, extraen los datos mediante comandos OC y los guardan en una carpeta, también
extraer información del grafana alojado en su cluster, mediante Screenshots. Luego de analizar este procedimiendo, se llego a la conclusión de que este 
procedimiento se podía ejecutar mediante un playbook, de manera que este playbook, vaya ejecutando las tareas que se hacen manualmente, para poder extraer
la información del cluster y ver el estado de este mismo.
</p>

	<h1 align="center"> Funcionalidad y estructura del producto </h1>
	
<p> La principal funcion del producto, es poder ejecutar y cumplir con las espectativas del healthcheck que se realiza diariamente, para eso, tomamos
como referencia el heathcheck manual que hay actualmente y en base a eso estructuramos el playbook, de manera que cada tarea que se ingrese en el playbook
corresponda a lo que se desea visualizar, guiandonos por el healthcheck manual que hay actualmente.
</p>

<p> Respecto a la funcionalidad del producto, actualmente se ejecuta localmente en una maquina Linux, dicha maquina linux debe contener los siguientes servicios:
	-Servicio ansible
	-Servicio gem
	-Servicio asciidoctor
	-Habilitación de comandos OC en la maquina.
	-Servicio jq
</p>

	<h3 align="center"> Uso y ejecución del playbook </h3>
	
<p> Luego de tener todos los servicios necesarios para la ejecución del playbook, se debe hacer lo siguiente:

	-Alojar la carpeta TTF en la raíz de la maquina que se ejecutará el playbook.
	-Comandos para la ejecución del playbook y conversión a PDF.
		-ansible-playbook <nombre_playbook>
		-asciidoctor-pdf <nombre_archivo.adoc> (alojado en la carpeta Documentation)
</p>

	<h4 align="center"> Referencias y documentación </h4>
<p> 
<a href="https://docs.ansible.com/ansible/latest/index.html"> Documentación oficial modulo ansible </a> 
<a href="https://docs.asciidoctor.org/pdf-converter/latest/convert-to-pdf/"> Conversión de archivo .adoc a PDF, con modulo asciidoctor </a>
</body>
