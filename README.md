# DinnerSoft

    README.txt             ADSI ANALISIS Y DESARROLLO DE SISTEMAS DE INFORMACION
                                   DINNERSOFT


    La carpeta contiene los siguientes archivos:
    ===========================================



    -README.txt : este archivo.
    -Documentacion: este archivo contiene informacion de como se implemento la solucion de la tarea, esta
                    explicacion se realiza norma IEEE y diagramacion.
    -mibackup : script con la solucion de nuestro proyecto.
    -Proyecto : programa como tal y funcionando.                   



    Para ejecutar el script:
    =======================

    - Otorgue permiso de ejecucion al archivo mibackup.
    - luego en el directorio en que se encuentra el script ejecute:
      ./mibackup <camino completo del directorio a copiar> [lista de extensiones]

        Nota:
	====
	Es importante poner el camino completo en el argumento 1 , ademas no debe terminar con el caracter "/"
	ejemplo:
	si se desea realizar un backup del directorio restaurant situado en el directorio raiz del usuario se debe ejecutar:

	$./mibackup /home/..../usuario/restaurant *.c *.txt *.jpg
    
    - El archivo de salida es enviado al directorio creado $HOME/mibacKup

    - Para descomprimir el archivo creado :
    $gzip -d archivo.tgz
    $tar -xf archivo.tar




    Para ejecutar el programa:
    =======================

    -descarge o ejecute el index.
    -pruebe y descubra las funcionalidades del ejecutable.




     Limitaciones conocidas:
     ======================

     -El script tiene problemas con archivos o directorios que poseen nombres que contengan espacios.
     -Producto de la implementacion de la copia del arbol de directorios, es posible tener directorios que se encuentren
      vacios, estos se borran pero a partir del segundo     nivel de profundidad es decir si es que existe un directorio vacio
      en el directorio principal este se mantendra  y sera incluido en archivo comprimido .
