# Primer Trabajo de Ingenieria de Software 3 - Git Básico

Este trabajo fue hecho para realizar la primera asignatura de la materia.

### 4- Desarrollo:

#### 1- Instalar Git
Los pasos y referencias asumen el uso del sistema operativo Windows, en caso otros SO seguir recomendaciones específicas.

  - Bajar e instalar el cliente git. Por ejemplo, desde https://git-scm.com/
  - Bajar e instalar un cliente visual. Por ejemplo, TortoiseGit para Windows o SourceTree para Windows/MAC:
    - https://tortoisegit.org/
    - https://www.sourcetreeapp.com/
    - Lista completa: https://git-scm.com/downloads/guis/

#### 2- Crear un repositorio local y agregar archivos
  - Crear un repositorio local en un nuevo directorio.
  ![Screenshot](Images/Image_01.png)
  ![Screenshot](Images/Image_02.png)
  - Agregar un archivo Readme.md, agregar algunas líneas con texto a dicho archivo.
  ![Screenshot](Images/Image_03.png)
  - Crear un commit y proveer un mensaje descriptivo.
  ![Screenshot](Images/Image_04.png)

#### 3- Crear un repositorio remoto
  - Crear una cuenta en https://github.com
  ![Screenshot](Images/Image_05.png)
  (Ya tenia uno, estoy usando mi git de proyectos personales)
  - Crear un nuevo repositorio en dicha página (vacío)
  ![Screenshot](Images/Image_06.png)
  - Asociar el repositorio local creado en el punto 2 al creado en github.
  ![Screenshot](Images/Image_07.png)
  - Subir los cambios locales a github.

#### 4- Familiarizarse con el concepto de Pull Request
Para algunos de los puntos proveer imágenes.

  - Explicar que es un pull request.
  ![Screenshot](Images/Image_08.png)
  
  Cuando hacemos una pull request, empezamos haciendo un fork, una copia de cierta branch que pasamos a controlar nosotros, la pull request es un pedido de unificar este fork al branch original con los nuevos cambios. Esto es evaluado por el propietario(s) original.
  
  - Crear un branch local y agregar cambios a dicho branch. 
  ![Screenshot](Images/Image_09.png)
  - Subir el cambio a dicho branch y crear un pull request.
  ![Screenshot](Images/Image_10.png)
  ![Screenshot](Images/Image_11.png)
  ![Screenshot](Images/Image_12.png)
  - Completar el proceso de revisión en github y mergear el PR al branch master.
  ![Screenshot](Images/Image_13.png)
  ![Screenshot](Images/Image_14.png)

#### 5- Mergear código con conflictos
  - Instalar alguna herramienta de comparación. Idealmente una 3-Way:
    - P4Merge https://www.perforce.com/downloads/helix-visual-client-p4v:
![alt text](p4merge.png)
    - Se puede omitir registración. Instalar solo opción Merge and DiffTool.

- ByondCompare trial version https://www.scootersoftware.com/download.php
  - Configurar Tortoise/SourceTree para soportar esta herramienta.
    - https://www.scootersoftware.com/support.php?zz=kb_vcs
    - https://medium.com/@robinvanderknaap/using-p4merge-with-tortoisegit-87c1714eb5e2
  - Clonar en un segundo directorio el repositorio creado en github.
  ![Screenshot](Images/Image_15.png)
  - En el clon inicial, modificar el Readme.md agregando más texto.
  ![Screenshot](Images/Image_16.png)
  - Hacer commit y subir el cambio a master a github.
  - En el segundo clon también agregar texto, en las mismas líneas que se modificaron el punto anterior.
  - Intentar subir el cambio, haciendo un commit y push. Mostrar el error que se obtiene.
  ![Screenshot](Images/Image_17.png)
  - Hacer pull y mergear el código (solo texto por ahora), mostrar la herramienta de mergeo como luce.
  ![Screenshot](Images/Image_18.png)
  - Resolver los conflictos del código.
  - Explicar las versiones LOCAL, BASE y REMOTE.
  
  La versión Local es aquella que tenemos nosotros, la Base es aquella de la cual dependen las versiones en conflicto, y la Remote la que esta remotamente generando los conflictos con la local al intentar pushearla.
  
  
  - Pushear el cambio mergeado.
  ![Screenshot](Images/Image_19.png)

#### 6- Algunos ejercicios online
  - Entrar a la página https://learngitbranching.js.org/
  - Completar los ejercicios **Introduction Sequence**
  ![Screenshot](Images/Image_20.png)
  - Opcional - Completar el resto de los ejercicios para ser un experto en Git!!!

#### 7- Crear Repositorio de la materia
  - Crear un repositorio para la materia en github. Por ejemplo **ing-software-3**
  - Subir archivo(s) .md con los resultados e imágenes de este trabajo práctico. Puede ser en una subcarpeta **trabajo-practico-01**
