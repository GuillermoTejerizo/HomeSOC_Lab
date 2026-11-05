# Poryecto HomeSOC_Lab
El objetivo de este proyecto es ir montar la estructura de una empresa y sus funciones. Quiero hacer que tenga funcionalidades basicas para que una empresa funcione.

## Objetivos
1. **ESTRUCTURA:** Voy a crear una estructura de directorios para los distintos departamentos y grupos de usuarios.
2. **AUTOMATIZAR:** Para ello voy a desarrollar scripts que automaticen el alta, baja y modificacion de usuarios, donde se les asignara un grupo y un departamento sin necesidad de tener que crear a los usuarios a mano.
3. **SEGURIDAD:** Quiero hacer un SOC con un SIEM desde el que monitorizar y seguir un registro de incidencias relacionadas con los inicios de sesion de los usuarios y los eventos del Domino. Ademas, quiero hacer auditorias y aniadir un Bastion.
4. **GESTION:** Para poder gestionar voy a implementar dos cosas: la primera Active Directory para el dominio de la empresa, y la segunda es un DNS que resuelva la busqueda del nombre del dominio.

## Fases
1. **Directorio:** AC DC, DNS, OU, grupos y red aislada.
2. **Autmatizacion:** scripts de alta, baja y cambios; lista de empleados (CSV); auditoria de grupos y ACL.
3. **Linux y Bastion:** unir un cliente Linux al dominio y usar otro servidor Linux como Bastion Host por SSH. Usar Apache para acceso desde navegador.
4. **SOC:** Enviar eventos del Dominio y Linux; crear y validar alertas.
5. **Crecimiento:** Inucluir un cliente Windows, un segundo DC para deundancia y segmentacion de la red.

## Estructura de la documentacion
```
HomeSOC --> README.md
    |
    |---> Arquitectura
    |           |
    |           |-> README.md
    |
    |---> Directori0
    |       |
    |       |--> README.md
    |       |--> Imagenes
    |
    |---> Automatizacion
    |       |
    |       |--> README.md
    |       |--> Documentos
    |       |           |--> Scripts
    |       |           |--> CSV
    |       |
    |       |-->Imagenes
    |
    |---> Linux_Bastion
    |           |
    |           |--> README.md
    |           |--> Imagenes
    |
    |---> SOC
    |      |
    |      |--> README.md
    |      |--> Imagenes
    |
    |---> Crecimiento
                |
                |--> Cliente Windows
                |           |
                |           |-> README.md
                |           |-> Imagenes
                |
                |--> Dominio secundario
                |           |
                |           |-> README.md
                |           |-> Imagenes
                |
                |--> Segmentacion de red
                            |
                            |-> README.md
```