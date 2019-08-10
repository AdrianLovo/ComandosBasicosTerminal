
# Lista de comandos Basicos Linux

## 1. NAVEGACION ENTRE ARCHIVOS Y LISTADO DE ARCHIVOS
	
	Limpiar pantalla
		> clear | Ctrl + l

	Donde nos encontramos en directorio
		> pwd	
		> cd + enter (Por defecto nos lleva a home)

	Listar archivos
		> ls
		> ls -l
			"-" para los archivos
			"d" para directorios
			"a" indica un link
		> ls -lt (indica la fecha de creacion)
		> ls -ltr (Ordena por el ultimo creado)
		> ls -lh (Muestra el tamaño de los archivos en un formato legible)
		> ls -lhsr (Archivo ordenados segun tamaño)

	Listar directorios y mostrar el tamaño
		> du -h -d 1	

	Cambio de directorio
		> cd (Change Directory)		


## 2. CREACION DE DIRECTORIOS, MOVER COPIAR Y ELIMINAR ARCHIVOS
	
	Crear Directorio
		> mkdir NombreCarpeta

	Mover archivos
		> mv NombreArchivo.terminacion Carpeta/
		> mv ../NombreArchivo.terminacion ./	(Mover archivo de directorio padre)
		> mv ../*terminacion .					(Mover todos los archivos de un tipo al directorio actual)

	Copiar Archivos
		> cp NombreArchivo.terminacion RutaDirectorio

	Renombrar Archivos
		> mv NombreArchivo.terminacion NombreNuevo.terminacion

	Modificar archivo
		> touch NombreArchivo 	(Modifica la fecha de ultimo acceso y modificacion a el archivo)


## 3. LINKS (Apuntadores)
		
	Crear un link
		> ln -s Original Nuevo

	Eliminar archivos y carpetas
		> rm nombre
		> rm -rf Carpeta/

## 4. Otros comandos		
	
	Informacion sobre comandos
		> man "COMANDO"		

	Calculadora en terminal
		> bc -q (Calculador), exit(quit)

	Leer archivo
		> more nombreArchivo
		> tail -f nombreArchivo (Ultimas lienas modificadas)
		> cat nombreArchivo (Muestra todo el archivo)
		> wc -l nombreArchivo (Lineas que posee el archivo)


## 5. Monitoreo de Procesos

	Ruta de comando que se esta ejecutando
		> which comando
		> top (Monstra listado de procesos)
		> php archivo.php & (Envia al background de la terminal y regresa el PID)
		> kill -9 PID


## 6. Busqueda de contenido
	
	Dentro de un archivo segun una palabra
		> cat nombreArchivo | grep palabra
		> cat nombreArchivo | grep palabra | wc -l (Indicar unicamente el numero de coincidencias)


	Dentro de un directorio (Indicando el archivo)
		> grep -r . -e palabraBuscar	(. indica el directorio actual)
		> grep -r . -e palabraBuscar -n	(. indica el directorio actual, indica tambien la linea de coincidencia)

## 7. Crontab
	
	Mostrar
		> crontab -l 

	Editar
		> crontab -e


	Minutos (0-59) / Horas (0-23) / Dia del mes (1-31) / Mes (1-12) / dia de la semana (0 Domingo - 6 Sabado) / 

	* * * * * script.sh

	* 		:Todos los valores
	1-10 	:De 1 a 10
	*/5 	:Cada 5 minutos








	











