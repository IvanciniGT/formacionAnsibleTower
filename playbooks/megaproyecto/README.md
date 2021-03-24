Proceso en IT dentro de ITNOW

Despliegue de una maquina virtual... 2
    Aprovisionamiento de una nueva app en un nuevo entorno
    - Linux - Servidor de aplicaciones - Instalar una app
    - Linux - BBDD - Ejecutar unos scripts de base de datos

RESTAURAR INVENTARIO >>>>> 1 >>>> 3 >>>>>>>>>>>>> |
                                                  | 6  >>> 7 >>>> 8 >>> TODO GUAY
                           2 >>>> 4 >>>> 5 >>>>>> |               V
                                                         A restablecer todo como estaba


1º Preparar mi máquina del servidor de aplicaciones
    - Actualizar SO
    - Dendendencias 
    - Configuraciones SO... Variables SO... Usuarios... Net
2º Preparar mi máquina del servidor de BBDD
    - Actualizar SO
    - Dendendencias 
    - Configuraciones SO... Variables SO... Usuarios... Net
3º Instalar Servidor de Aplciaciones
    - Descargarlo... Actualizar unos repos
    - Instalarlo
    - Configurarlo
    - Arrancarlo
4º Instalar Servidor de BBDD
    - Descargarlo... Actualizar unos repos
    - Instalarlo
    - Configurarlo
    - Arrancarlo
5º Cargar datos y crear estructuras en la BBDD
    - Conectarme con BBDD
    - Crear estructuras
    - Crear datos
6º Montar app en el servidor de aplciaciones
    - Conectarme con Servidor de aplciaciones
    - Instalar app
7º Arrancar la app
    - Arrancar la app
8º Pruebas 
    - Probar conectividad BBDD
    - Probar conectividad con app
    - Smoke test app
    
SI PETAN LAS PRUEBAS
    0: Parada de la app
    A: Desmontar el chiringuito
        - Desinstalar app
    B: Borra BBDD
    C: Desinstalar BBDD
    D: Desinstalar Webserver
    