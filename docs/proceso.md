#### Documentación del proceso
 
 1. CLONACIÓN Y CREACIÓN DEL REPOSITORIO

    - Creamos una carpeta y desde vsc hacemos **git init** y **git clone del repositorio del profesor.** 

    - En vsc creamos .gitignore, metemos DS_Start y UD01_exam_IAW/, 
      **git add .gitignore** y **commit** para que esos archivos no nos molesten a la hora de hacer el ejercicio.

      Todo lo vamos comprobando con **git status**.

    - El enunciado pide copiar el enunciado a la carpeta principal con **cp UD02_exam_IAW/UD02_exam.md .**
      Añadimos y guardamos los cambios **git add .** y **git commit -m ""**

    - En vsc en el apartado de git, le damos a la nube con la flecha hacia arriba y seleccionamos github público.
      (crea el repo remoto de GitHub, conecta mi repo local y sube mi rama main a sus commits).

### **SÚPER IMPORTANTE PARA CREAR EL REPOSITORIO REMOTO** 
      Nube con flecha hacia arriba, seleccionar public.    



2. CREACIÓN Y GESTIÓN DE RAMAS

    - Creamos la rama documentación con **git checkout -b documentacion** (la crea y cambia directamente a ella), comprobamos git status.
    - Nos gestionamos las ramas con **git branch**.


3. CREACIÓN, GESTIÓN Y PUBLICACIÓN DEL PROJECTO MKDOCS 

  - Toca crear el proyecto MkDocs en la rama documentación, desde la carpeta principal **mkdocs new .**. Crea la estructura inicial de MkDocs en mi repo. Ahora aparecen los archivos docs/index.md y mkdocs.yml.

  - En el archivo yml, añadimos como los enlaces entre las diferentes páginas para que en mkdocs se reconozcan entre ellos. 

  site_name: Documentación de git

   nav:
    - Inicio: index.md
    - Comandos de Git: comandos.md
    - Proceso: proceso.md


  - Ejecutamos **mkdocs serve**, comprobamos que funciona bien por web y guardamos los cambios en la rama documentación con **git add docs/ mkdocs.yml**, comprobamos con git status y hacemos commit.
