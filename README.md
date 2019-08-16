# Internships Bootcamp
## Git
![Git and Github](http://blog.desafiolatam.com/wp-content/uploads/2016/05/git-github-logo.jpg)
### ¿Qué es Git?
+ Sistema de control distribuido.
+ Ayuda a coordinar los cambios en el proyecto.
+ Conoces quien hace los cambios y cuando los hizo.
+ Repositorios locales y remotos.
### Instalación
[Sitio oficial de git](https://git-scm.com/)

### Flujo de trabajo
Tu repositorio local esta compuesto por tres "árboles" administrados por git. El primero es tu `Directorio de trabajo` que contiene los archivos, el segundo es el `Index` que actua como una zona intermedia, y el último es el `HEAD` que apunta al último commit realizado. 

![Flujo de trabajo](https://rogerdudler.github.io/git-guide/img/trees.png)

### Comandos básicos
Para crear un repositorio basta con correr el siguiente comando
```
$ git init
```

Para pasar un archivo al stage area es necesario ingresar el siguiente comando
```
$ git add <file>
```

Para configurar el email del usuario de git basta con el siguiente comando
```
$ git config --global user.email
```

Y para configurar el nombre del usuario de git...
```
$ git config --global user.name
```

Si queremos ver el historial de commits hechos sobre el proyecto el comando `git log` lo muestra:
```
$ git log 
```

El comando `git status` te mostrará los diferentes estados de los archivos en tu working directory y stage area.
```
$ git status
```

El comando `commit` nos ayuda a crear una especie de snapshot o checkpoint de nuestro código.
```
$ git commit -m "Mi primer commit"
```


Para revertir los cambios habientes en el working directory:

```
$ git checkout --
```


Para ver las modificaciones hechas en los archivos desde el commit anterior y los nuevos:
```
$ git diff --
```

### Integración con Github
Para obtener un repositorio de github hay dos maneras, clonarlo mediante git o descargarlo del perfil, la diferencia entre ambas es que si se descarga se perderá la integración con git y se tendrá que gestionar de manera manual a diferencia de cuando se clona, se genera las configuraciones necesarias que permitirán usar git, para clonarlo es necesario el siguiente comando
```
$ git clone [url] [nombre de la carpeta a crear]
```

Para añadir un nuevo repositorio Git remoto, asignándole un nombre con el que referenciarlo fácilmente, ejecuta 
```
git remote add [nombre] [url]
```

Para bajar cambios que se encuentran en el repositorio remoto:
```
$ git pull origin [rama]
```

Para subir los cambios al repositorio: 
```
$ git push origin [rama]
```
