Laboratorio 05 
Tema: Django 
Profesor 	Escuela 	Asignatura
Prof. Anibal Sardon
a.sardon.unsa@gmail.com	Escuela Profesional de 
Ingeniería de Sistemas	Programación Web 2 
Semestre: III 
Código: 1702122

Laboratorio 	Tema 	Duración
05 	Django 	04 horas

Semestre académico 	Fecha de inicio 	Fecha de entrega
2023 - A 	05 Junio 2023 	12 Junio 2023

1. Competencias del curso 
General: C.c. Diseña responsablemente aplicaciones web, sus componentes o procesos para satisfacer necesidades dentro de restricciones realistas: económicas, medio ambientales, sociales, políticas, ´éticas, de salud, de seguridad, manufacturación y sostenibilidad. 
Específica: C.m. Construye responsablemente soluciones con tecnología web siguiendo un pro ceso adecuado llevando a cabo las pruebas ajustada a los recursos disponibles del cliente. 
Específica: C.p. Aplica de forma flexible técnicas, métodos, principios, normas, estándares y herramientas del desarrollo web necesarias para la construcción de aplicaciones web e implementación de estos sistemas en una organización. 
2. Resultado del estudiante 
RE. 2 La capacidad de aplicar diseño de ingeniería para producir soluciones a problemas y diseñar sistemas, componentes o procesos para satisfacer necesidades específicas dentro de consideraciones realistas en los aspectos de salud pública, seguridad y bienestar; factores globales, culturales, sociales, económicos y ambientales. 
RE. 8 La capacidad de crear, seleccionar y utilizar técnicas, habilidades, recursos y herramientas modernas de ingeniería y tecnologías de la información, incluyendo la predicción y el modela miento, con una comprensión de las limitaciones. 
3. Equipos, materiales y temas 
	Sistema Operativo (GNU/Linux de preferencia). 
	GNU Vim. 
	Python 3. 
	Git. 
	Cuenta en GitHub con el correo institucional. 
	Entorno virtual. 
	Django 4. 
4. Directorio de trabajo 
Cree su directorio de trabajo. 
Luego, diríjase a este directorio, para clonar su repositorio y continuar sus prácticas. 
Listing 1: Creando directorio de trabajo 
$ mkdir -p $HOME/rescobedoq/ 
Listing 2: Dirigiéndonos al directorio de trabajo 
$ cd $HOME/rescobedoq/ 
Listing 3: Clonando repositorio GitHub 
$ git clone [URL_DE_SU_GITHUB_PRIVADO] 
Listing 4: Creando directorio para laboratorio 
$ mkdir -p $HOME/rescobedoq/pw2-lab-23a/lab05/exercises/ 
Siempre evalúe utilizar el archivo. gitignore para no considerar algunos archivos innecesarios sobre todo para el repositorio GitHub. 
Puede haber varios de estos archivos y estar ubicados estratégicamente; por ejemplo solo para un laboratorio en particular. 
Listing 5: Creando. gitignore 
$ vim $HOME/rescobedoq/pw2-lab-23a/lab05/.gitignore 
Listing 6: Ejemplo de .gitignore 
my_env/bin/* 
my_env/lib/* 
my_env/src/__pycache__/* 
*.pyc 
Estudie el archivo .gitignore del proyecto Library : 
https://github.com/mdn/django-locallibrary-tutorial/blob/main/.gitignore 
5. Marco teórico 
5.1. Django 
Django es un framework web Python con el cual el desarrollo de sitios web son rápidos, seguros y sobre todo fáciles de mantener. 
Django se ocupa de gran parte de las molestias del desarrollo web, por lo que puede concentrarse en escribir su aplicación sin necesidad de reinventar la rueda. 
Es software libre, tiene una comunidad prospera y activa, excelente documentación y muchas opciones de soporte gratuito y de pago. 
5.2. Crear un directorio para el entorno virtual de Django Para crear un ambiente elija en que directorio se va crear el entorno virtual. 
Listing 7: Creando directorio para entorno virtual en Unix 
$ mkdir -p $HOME/rescobedoq/pw2-lab-23a/lab05/my_env 
Listing 8: Creando directorio para entorno virtual 
$ mkdir -p $HOME/rescobedoq/pw2-lab-23a/lab05/my_env 
5.3. Crear entorno virtual en un directorio 
En este directorio crear un entorno virtual ejecutando el siguiente comando: 
Listing 9: Creando entorno virtual en GNU/Linux 
$ cd $HOME/rescobedoq/pw2-lab-23a/lab05/my_env 
$ virtualenv -p python3 . 
Listing 10: Creando entorno virtual en MS Windows 
C:\>python -m venv c:\rescobedoq\pw2-lab-23a\lab05\my_env 
Listing 11: Creando entorno virtual en MacOS 
$ python -m venv $HOME/rescobedoq/pw2-lab-23a/lab05/my_env 
5.4. Activando entorno virtual 
En el directorio de trabajo active el entorno virtual ejecutando el script activate. 
Sea cual sea nuestro sistema operativo sabremos que el entorno virtual se ha activado porque su nombre aparece entre paréntesis delante del promt. 
Listing 12: Activando entorno virtual en GNU/Linux 
$ cd $HOME/rescobedoq/pw2-lab-23a/lab05/exercises/ 
$ source ./../my_env/bin/activate 
(my_env) user@localhost:$ 
Listing 13: Activando entorno virtual en GNU/Linux 
C:\rescobedoq\pw2-lab-23a\lab05\my_env\scripts\activate.bat 
Listing 14: Activando entorno virtual en GNU/Linux 
$ source $HOME/rescobedoq/pw2-lab-23a/lab05/my_env/bin/activate 
5.5. Desactivando entorno virtual 
El comando para desactivar el entorno virtual es idéntico para Windows, macOS y Linux: 
Listing 15: Desactivando entorno virtual 
$ deactivate 
5.6. Instalando Django dentro del entorno virtual 
Siempre hay que estar conscientes de los paquetes de nuestro entorno virtual. 
Listing 16: Mostrando paquetes instalados en el entorno virtual 
(my_env) user@localhost:$ pip list 
Package Version 
---------- ------- 
pip 22.0.4 
setuptools 62.1.0 
wheel 0.37.1 
Instalamos Django con pip: 
Listing 17: Instando Django 
(my_env) user@localhost:$ pip install Django 
Volvemos a listar los paquetes instalados: 
Listing 18: Mostrando Django instalado en el entorno virtual 
(my_env) user@localhost:$ pip list 
Package Version 
---------- ------- 
asgiref 3.5.2 
Django 4.0.5 
pip 22.0.4 
setuptools 62.1.0 
sqlparse 0.4.2 
wheel 0.37.1 
6. Ejercicios 
Cree la aplicación Library paso a paso desde la siguiente url: 
https://developer.mozilla.org/en-US/docs/Learn/Server-side/Django/Tutorial_local_ library_website 
capturas de pantalla:
 
 
7. Tarea 
Elabore un primer informe grupal de la aplicación que desarrollara durante este semestre. Utilicen todas las recomendaciones dadas en la aplicación library. 
Acuerdos: 
• Los grupos pueden estar conformado por 1 a 4 integrantes. 
• Solo se presenta un informe grupal. 
• Solo se revisa un repositorio. (El único que esté en el informe grupal). 
• Todos los integrantes del grupo tienen una copia del laboratorio e informe en su repositorio privado. 
• Todos los integrantes deben pertenecer al mismo grupo de laboratorio. 
• El docente preguntar en cualquier momento a un integrante sobre el proyecto, código fuente, avance. 
Github:
8. Pregunta 
Por cada integrante del equipo, resalte un aprendizaje que adquirió al momento de estudiar Django. No se reprima de ser detallista. Coloque su nombre entre paréntesis para saber que es su aporte. 
9. Entregables 
El informe debe tener un enlace al directorio específico del laboratorio en su repositorio GitHub privado donde esté todo el código fuente y otros que sean necesarios. Evitar la presencia de archi vos: binarios, objetos, archivos temporales, cache, librerías, entornos virtuales. Si hay configuraciones particulares puede incluir archivos de especificación como: requirements.txt, o leeme.txt. 
No olvide que el profesor debe ser siempre colaborador a su repositorio (Usuario del profesor @rescobedoq). 
Para ser considerado con la calificación de máxima nota, el informe debe estar elaborado en latex 
Usted debe describir solo los commits más importantes que marcaron hitos en su trabajo, adjuntando capturas de pantalla, del commit, del código fuente, de sus ejecuciones y pruebas. 
En el informe siempre se debe explicar las imágenes (código fuente, capturas de pantalla, commits, ejecuciones, pruebas, etc.) con descripciones puntuales pero precisas. 
10. Rubricas 
10.1. Rubrica para entregable Informe 
Tabla 1: Rubrica para tipo de Informe 
Informe 	Cumple 	No 
cumple
Latex 	El informe está en formato PDF desde Látex, con un formato limpio (buena presentación) y fácil de leer.	20 	0
Mark Down 	El informe está en formato PDF desde Mark Down README.md, con un formato limpio (buena pre sensación) y fácil de leer.	17 	0
MS Word 	El informe está en formato PDF desde plantilla MS Word, con un formato limpio (buena presentación) y fácil de leer.	15 	0
Observaciones 	Por cada observación se le descontar ‘a puntos. 	- 	-

10.2. Rubrica para el contenido del Informe y demostración 
El alumno deberá marcar o dejar en blanco en las celdas de la columna Checklist, de acuerdo a si cumplió o no con el ítem correspondiente. 
Si un alumno supera la fecha de entrega, su calificación siempre será sobre la nota mínima aprobada, siempre y cuando cumpla con todos lo ítems. 
El alumno debe autocalificarse en la columna Estudiante de acuerdo a la tabla de calificación de niveles de desempeño: 
Tabla 2: Niveles de desempeño 
Nivel
Puntos 	Insatisfactorio 25 % 	En Proceso 50 % Satisfactorio 75 % Sobresaliente 100 % 
2.0		0.5 			1.0 		1.5 			2.0 
4.0 		1.0 			2.0 		3.0 			4.0 
Tabla 3: Rubrica para contenido del Informe y demostración 
Contenido y demostración 	Puntos 	Checklist	Estudiante 	Profesor
1. GitHub 	Hay enlace URL activo del directorio para el laboratorio hacia su repositorio GitHub con código fuente terminado y fácil de revisar.	2			
2. Commits 	Hay capturas de pantalla de los commits más importantes con sus explicaciones detalladas. (El profesor puede preguntar para refrendar calificación).	4			
3. Código fuente	Hay porciones de código fuente importantes con numeración y explicaciones detalladas de sus funciones.	2			
4. Ejecución 	Se incluyen ejecuciones/pruebas del código fuente explicadas gradualmente.	2			
5. Pregunta 	Se responde con completitud a la pregunta formulada en la tarea. (El profesor puede preguntar para refrendar calificación).	2			
6. Fechas 	Las fechas de modificación del código fuente están dentro de los plazos de fecha de entrega establecidos.	2			
7. Ortografía 	El documento no muestra errores ortográficos. 	2			
8. Madurez 	El Informe muestra de manera general una evolución de la madurez del código fuente, explicaciones puntuales pero precisas y un acabado impecable. (El profesor puede preguntar para refrendar calificación).	4			
Total 	20			

11. Referencias 
https://developer.mozilla.org/en-US/docs/Learn/Server-side/Django/Tutorial_local_ library_website 
https://github.com/mdn/django-locallibrary-tutorial 
https://github.com/rescobedoq/pw2/tree/main/labs/lab05 
William S. Vincent. (2022). Django for Beginners: Build websites with Python. Django 4.0. leanpub.com. [URL] 
