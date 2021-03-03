![](https://cafam.edu.do/media/rc4jfl2l/cafam-logo2.png)
## El Uso de Git y GitHub para trabajos colaborativos.<br><br>

# ***Participantes***

### 1-*Raymond Sandoval* #1<br><br>
### 2-*Francisco Garcia* #9<br><br>
### 3-*Shawn Diaz* #8<br><br>
<br>

## **Git**

![git dick](https://julioecheverri.files.wordpress.com/2016/07/git-logo.png)
<br>
<br>
<br>
## **Git Hub**
![](https://github.githubassets.com/images/modules/logos_page/GitHub-Mark.png)
<br>
<br>
# ***Contenidos***

* Introduccion
* Desarrollo
* Comandos Utilizados
* Imagenes Relacionadas
* Conclusion
* Bibliografia
<br>
<br>
 # ***Introduccion***
En este proyecto se hablara sobre el software de control de versiones y host de internet github, explicando la funcion y flujo de trabajo de cada uno,  distribuyendo los contenids en un indice de anera organizada, con codigos de ejemplo, imagenes relacionadas y la bibliografia con los links correspondientes a cada pagina utilizada para utilizar su informacion
<br><br>
# ***Temas Desarrollados*** <br>
## **Que es git?**
Es un software de control de versiones diseñado por Linus Torvalds, pensando en la eficiencia, la confiabilidad y compatibilidad del mantenimiento de versiones de aplicaciones cuando éstas tienen un gran número de archivos de código fuente. Su propósito es llevar registro de los cambios en archivos de computadora incluyendo coordinar el trabajo que varias personas realizan sobre archivos compartidos en un repositorio de código<br>

## **Caracteristicas:**<br>
- Fuerte apoyo al desarrollo no lineal, por ende rapidez en la gestión de ramas y mezclado de diferentes versiones.<br> 
- Gestión distribuida.<br>
- Los almacenes de información pueden publicarse por HTTP, FTP, rsync o mediante un protocolo nativo <br>
- Los repositorios Subversion y svk se pueden usar directamente con git-svn.<br>
- Gestión eficiente de proyectos grandes, dada la rapidez de gestión de diferencias entre archivos, entre otras mejoras de optimización de velocidad de ejecución.<br>
- Realmacenamiento periódico en paquetes<br>
- Todas las versiones previas a un cambio determinado, implican la notificación de un cambio posterior en cualquiera de ellas a ese cambio<br>
- Resulta algo más caro trabajar con ficheros concretos frente a proyectos<br>
- Los renombrados se trabajan basándose en similitudes entre ficheros <br>
- Compatibilidad con Github y Microsoft Visual Studio Code

## **Flujo de Trabajo** <br>

Git plantea una gran libertad en la forma de trabajar en torno a un proyecto. Sin embargo, para coordinar el trabajo de un grupo de personas en torno a un proyecto es necesario acordar como se va a trabajar con Git. A estos acuerdos se les llama flujo de trabajo
Los flujos de trabajo más populares son git-flow, GitHub-flow, GitLab Flow y One Flow<br>
<br>
![](https://zepel.io/blog/content/images/2020/05/GitFlow-git-workflow-2.png)<br>

#### **Master**
Es la rama principal. Contiene el repositorio que se encuentra publicado en producción, por lo que debe estar siempre estable.<br>

#### **Development**
Es una rama sacada de Master. Es la rama de integración, todas las nuevas funcionalidades se deben integrar en esta rama. Luego que se realice la integración y se corrijan los errores (en caso de haber alguno), es decir que la rama se encuentre estable, se puede hacer un merge de development sobre la rama Master.<br>

#### **Features**
Cada nueva funcionalidad se debe realizar en una rama nueva, específica para esa funcionalidad. Estas se deben sacar de Development. Una vez que la funcionalidad esté desarrollada, se hace un merge de la rama sobre Development, donde se integrará con las demás funcionalidades.<br>

#### **Hotfix**
Son errores de software que surgen en producción, por lo que se deben arreglar y publicar de forma urgente. Es por ello, que son ramas sacadas de Master. Una vez corregido el error, se debe hacer una unificación de la rama sobre Master. Al final, para que no quede desactualizada, se debe realizar la unificación de Master sobre Development.<br>

#### **Release**
Las ramas de release apoyan la preparación de nuevas versiones de producción. Para ellos se arreglan muchos errores menores y se preparan adecuadamente los metadatos. Se suelen originar de la rama develop y deben fusionarse en las ramas master y develop.<br><br>

## **Que es GitHub** <br>
Es una forja para alojar proyectos utilizando el sistema de control de versiones Git. Se utiliza principalmente para la creación de código fuente de programas de ordenador. El software que opera GitHub fue escrito en Ruby on Rails. Desde enero de 2010, GitHub opera bajo el nombre de GitHub, Inc. Anteriormente era conocida como Logical Awesome LLC. El código de los proyectos alojados en GitHub se almacena típicamente de forma pública.<br>
## **Caracteristicas:**<br>
- Wiki para cada proyecto.<br>
- Página web para cada proyecto.<br>
- Gráfico para ver cómo los desarrolladores trabajan en sus repositorios y bifurcaciones del proyecto.<br>
- Funcionalidades como si se tratase de una red social, por ejemplo, seguidores.<br>
- Herramienta para trabajo colaborativo entre programadores.<br>
- Gestor de proyectos de estilo Kanban.<br>
Actions herramientas de CI<br>
- Codespaces un IDE en la nube para los repositorios.<br>
- Colaboración para todos.<br>
## **Flujo de trabajo de Git Hub**<br>
![](https://res.cloudinary.com/practicaldev/image/fetch/s--M_fHUEqA--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://thepracticaldev.s3.amazonaws.com/i/128hsgntnsu9bww0y8sz.png)<br>
Este flujo es similar al flujo de *Git*, con la diferencia que para poder integrar la rama de funcionalidad en la que se está trabajando, se debe pasar por un Administrador de Integración quien es a su vez el encargado de integrar los cambios a la rama protegida Master.<br><br>

# ***Comandos utilizados con ejemplo***<br>
## ***Git & Git Hub:***<br>
    git help<br>

Muestra una lista con los comandos más utilizados en GIT.<br>

    git init<br>

Podemos ejecutar ese comando para crear localmente un repositorio con GIT y así utilizar todo el funcionamiento que GIT ofrece.<br>

    git add + path<br>

Agrega al repositorio los archivos que indiquemos.<br>

    git add -A<br>

Agrega al repositorio TODOS los archivos y carpetas que estén en nuestro proyecto, los cuales GIT no está siguiendo.<br>

    git commit -m "mensaje" + archivos<br>

Hace commit a los archivos que indiquemos, de esta manera quedan guardados nuestras modificaciones.<br>

    git commit -am "mensaje"<br>

Hace commit de los archivos que han sido modificados y GIT los está siguiendo.<br>

    git checkout -b NombreDeBranch<br>

Crea un nuevo branch y automaticamente GIT se cambia al branch creado, clonando el branch desde donde ejecutamos el comando.<br>

    git branch<br>

Nos muestra una lista de los branches que existen en nuestro repositorio.<br>

    git checkout NombreDeBranch<br>

Sirve para moverse entre branches, en este caso vamos al branch que indicamos en el comando.<br>

    git merge NombreDeBranch<br>

Hace un merge entre dos branches, en este caso la dirección del merge sería entre el branch que indiquemos en el comando, y el branch donde estémos ubicados.<br>

    git status<br>

Nos indica el estado del repositorio, por ejemplo cuales están modificados, cuales no están siendo seguidos por GIT, etc.<br>

    git clone URL/name.git NombreProyecto<br>

Clona un proyecto de git en la carpeta NombreProyecto.<br>

    git push origin NombreDeBranch<br>

Luego de que hicimos un git commit, si estamos trabajando remotamente, este comando va a subir los archivos al repositorio remoto, específicamente al branch que indiquemos.<br>

    git pull origin NombreDeBranch<br>

Hace una actualización en nuestro branch local, desde un branch remoto que indicamos en el comando.<br>
