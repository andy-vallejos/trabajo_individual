# TRABAJO INDIVIDUAL

Andy Gildo Vallejos Bascope

## Clase 1

### Que es git?

Es un sistema de control de controles

### Instalacion

Para mi sistema operativo que es linux es el siguiente comando:

```
    sudo pacman -S git
```

### Sistema de puntuacion

![alt text](/public/image.png)

### Configuraciones basicas

![alt text](/public/image2.png)

### Git add

Git add mueve los cambios de la carpeta al staging area.

```
    git add nombre_del_archivo
```

### Git commit

Si git add es “preparar”, entonces git commit es “tomar una foto (snapshot)” de esos cambios.Si git add es “preparar”, entonces git commit es “tomar una foto (snapshot)” de esos cambios.

```
    git commit -m "mensaje descriptivo"
```

### Git push

git push sirve para subir tus commits al repositorio remoto.

```
    git push origin nombre_de_la_rama
```

## CLase 2

### Directorio de trabajo (Modificado)

Tu carpeta local, esta escribiendo codigo, pero Git aun no lo tiene asegurado.

#### Untracked

Sin seguimiento.

#### Modified

Es cuando GIT ya tiene una version previa y lo modificas o eliminas.

#### Git restore

Descarta la modificacion

```
    git restore <archivo>
```

#### .gitignore

Es un archivo que almacena archivos o directorios los cuales queremos q sean ignorados por git para evitar que sean trackeados.

### Stage Area (Preparado)

El area de espera, le dices a git lo que quieres guardar.

### Repositorio local ()

#### Git commit

Crea un punto de guardado

```
    git commit -m "mensaje"
```

#### Git reset

Vuelve al anterior commit

```
    git reset --sogt HEAD~1
```

### Git Status

Permite ver en que estado se encuentran los archivos.

```
    git status
```

### Git log

Muestra todos los commits creados

```
    git log
```

![alt text](/public/image3.png)

### BUENAS PRACTICAS

Verbos imperativos
No usar punto final
Descriptivos
Usar como maximo 50 caracteres
![alt text](/public/image4.png)
