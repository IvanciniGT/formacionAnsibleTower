# formacionAnsibleTower

Funcionalidades que aporta AWX/Tower
- Automatizar el lanzamiento de playbooks
- Automatizar la carga de Inventarios
- Unificar ficheros de inventario
- Historico de operaciones sobre cada servidor
- Ejecución parametrizada de playbooks por dummies
- MultiTenance >>> 1 instalación, varias organizaciones
- Autenticación / Autorización de usuarios
- Repositorio de playbooks/inventario <<<< Repo GIT 
- Ejecución remota/centralizada HTTPs:
    - consola WEB
    - API REST <<< Programas que pueda ejecutar acciones ansible



Que cosas me faltan en AWX/Tower
- Planificación muy pobre "básica" de tareas 
    - Basada en CRON / temporizadores... FECHAS RIGIDAS
        Devops >>> CI/CD
        Terraform >>> Alquilan en automatico unas máquinas en AWS
            VVVVV
        Y después quiero ejecutar en ellas unos playbooks


                             Terraform 
                                VVV
Inventario >>> Source >>>> Amazon EC2 


Jenkins >>>> Orquestador de tareas DE TODO TIPO
    VVV
    AWX     >>>> Orquestador de tareas ansible

Terraform Provee          Provider      Proveer infraestructura
        VVVV
Ansible   Aprovisiona     Provisioner   Aprovisiona infraestructura --- TOMCAT
                                                                    --- MySQL
        VVVV
Instale una app 

    En Tomcat montar un WAR (que tengo que compilar previamente)
    En MySQL crear unas tablas de BBDD