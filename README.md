# Introducción al producto y su función dentro del proyecto

## Healthcheck automatizado mediante un playbook

La idea de hacer un healthecheck automatizado mediante un playbook, nace de la raiz en donde el cliente, en este caso Banco Pichincha, ejecuta  un healthcheck diario a mano, lo que quiere decir es que ingresan al cluster, extraen los datos mediante comandos OC y los guardan en una carpeta, también extraer información del grafana alojado en su cluster, mediante Screenshots. Luego de analizar este procedimiendo, se llego a la conclusión de que este  procedimiento se podía ejecutar mediante un playbook, de manera que este playbook, vaya ejecutando las tareas que se hacen manualmente, para poder extraer la información del cluster y ver el estado de este mismo.


### Funcionalidad y estructura del producto

La principal funcion del producto, es poder ejecutar y cumplir con las espectativas del healthcheck que se realiza diariamente, para eso, tomamos como referencia el heathcheck manual que hay actualmente y en base a eso estructuramos el playbook, de manera que cada tarea que se ingrese en el playbook corresponda a lo que se desea visualizar, guiandonos por el healthcheck manual que hay actualmente.

Respecto a la funcionalidad del producto, actualmente se ejecuta localmente en una maquina Linux, dicha maquina linux debe contener los siguientes servicios:
* [Ansible]([http://www.dropwizard.io/1.0.2/docs](https://www.digitalocean.com/community/tutorials/how-to-install-and-configure-ansible-on-ubuntu-20-04-es)/) - Instalación modulo ansible
* [Maven](https://maven.apache.org/) - Manejador de dependencias
* [ROME](https://rometools.github.io/rome/) - Usado para generar RSS

### Instalación 🔧

_Una serie de ejemplos paso a paso que te dice lo que debes ejecutar para tener un entorno de desarrollo ejecutandose_

_Dí cómo será ese paso_

```
Da un ejemplo
```

_Y repite_

```
hasta finalizar
```

_Finaliza con un ejemplo de cómo obtener datos del sistema o como usarlos para una pequeña demo_

## Ejecutando las pruebas ⚙️

_Explica como ejecutar las pruebas automatizadas para este sistema_

### Analice las pruebas end-to-end 🔩

_Explica que verifican estas pruebas y por qué_

```
Da un ejemplo
```

### Y las pruebas de estilo de codificación ⌨️

_Explica que verifican estas pruebas y por qué_

```
Da un ejemplo
```

## Despliegue 📦

_Agrega notas adicionales sobre como hacer deploy_

## Construido con 🛠️

_Menciona las herramientas que utilizaste para crear tu proyecto_

* [Dropwizard](http://www.dropwizard.io/1.0.2/docs/) - El framework web usado
* [Maven](https://maven.apache.org/) - Manejador de dependencias
* [ROME](https://rometools.github.io/rome/) - Usado para generar RSS

## Contribuyendo 🖇️

Por favor lee el [CONTRIBUTING.md](https://gist.github.com/villanuevand/xxxxxx) para detalles de nuestro código de conducta, y el proceso para enviarnos pull requests.

## Wiki 📖

Puedes encontrar mucho más de cómo utilizar este proyecto en nuestra [Wiki](https://github.com/tu/proyecto/wiki)

## Versionado 📌

Usamos [SemVer](http://semver.org/) para el versionado. Para todas las versiones disponibles, mira los [tags en este repositorio](https://github.com/tu/proyecto/tags).

## Autores ✒️

_Menciona a todos aquellos que ayudaron a levantar el proyecto desde sus inicios_

* **Andrés Villanueva** - *Trabajo Inicial* - [villanuevand](https://github.com/villanuevand)
* **Fulanito Detal** - *Documentación* - [fulanitodetal](#fulanito-de-tal)

También puedes mirar la lista de todos los [contribuyentes](https://github.com/your/project/contributors) quíenes han participado en este proyecto. 

## Licencia 📄

Este proyecto está bajo la Licencia (Tu Licencia) - mira el archivo [LICENSE.md](LICENSE.md) para detalles

## Expresiones de Gratitud 🎁

* Comenta a otros sobre este proyecto 📢
* Invita una cerveza 🍺 o un café ☕ a alguien del equipo. 
* Da las gracias públicamente 🤓.
* Dona con cripto a esta dirección: `0xf253fc233333078436d111175e5a76a649890000`
* etc.



---
⌨️ con ❤️ por [Villanuevand](https://github.com/Villanuevand) 😊
