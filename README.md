# Introducción al producto y su función dentro del proyecto

## Healthcheck automatizado mediante un playbook

La idea de hacer un healthecheck automatizado mediante un playbook, nace de la raiz en donde el cliente, en este caso Banco Pichincha, ejecuta  un healthcheck diario a mano, lo que quiere decir es que ingresan al cluster, extraen los datos mediante comandos OC y los guardan en una carpeta, también extraer información del grafana alojado en su cluster, mediante Screenshots. Luego de analizar este procedimiendo, se llego a la conclusión de que este  procedimiento se podía ejecutar mediante un playbook, de manera que este playbook, vaya ejecutando las tareas que se hacen manualmente, para poder extraer la información del cluster y ver el estado de este mismo.


### Funcionalidad y estructura del producto

La principal funcion del producto, es poder ejecutar y cumplir con las espectativas del healthcheck que se realiza diariamente, para eso, tomamos como referencia el heathcheck manual que hay actualmente y en base a eso estructuramos el playbook, de manera que cada tarea que se ingrese en el playbook corresponda a lo que se desea visualizar, guiandonos por el healthcheck manual que hay actualmente.

Respecto a la funcionalidad del producto, actualmente se ejecuta localmente en una maquina Linux, dicha maquina linux debe contener los siguientes servicios:
* [Ansible](https://www.digitalocean.com/community/tutorials/how-to-install-and-configure-ansible-on-ubuntu-20-04-es) - Instalación modulo ansible
* [Gem](https://howtoinstall.co/es/gem) - Instalación servicio gem
* [Asciidoctor-pdf](https://docs.asciidoctor.org/pdf-converter/latest/install/) - Instalación de asciidoctor-pdf con modulo gem
* [jq](https://howtoinstall.co/es/jq) - Instalación servicio JQ
* [Modulo OC](https://docs.openshift.com/container-platform/4.8/cli_reference/openshift_cli/getting-started-cli.html) - Instalación OC cli en maquina local

### Uso y Ejecución del playbook 

Luego de tener todos los servicios necesarios para la ejecución del playbook, se debe hacer lo siguiente:

_Ejecutar los siguientes comandos_

```
ansible-playbook <nombre_playbook>
```
```
asciidoctor-pdf <nombre_archivo.adoc> (alojado en la carpeta documentation)
```
También se debe tener en cuenta, que la carpeta TTF, debe estar alojada en la raíz de la maquina donde se va ejecutar el playbook.

### Referencias y documentación relacionada al playbook ⚙️

_Documentación_
* [Documentación oficial modulo ansible](https://docs.ansible.com/ansible/latest/index.html)
* [Conversión de archivo .adoc a PDF, con modulo asciidoctor](https://docs.asciidoctor.org/pdf-converter/latest/convert-to-pdf/)

