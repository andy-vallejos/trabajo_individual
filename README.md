# TRABAJO INDIVIDUAL

Andy Gildo Vallejos Bascope

## Clase 1

### Que es git?

Es un sistema de control de controles

### Instalacion

Para mi sistema operativo que es linux es el siguiente comando:

````
    sudo pacman -S git
````

### Sistema de puntuacion

![alt text](/public/image.png)

### Configuraciones basicas

![alt text](/public/image2.png)

### Git add

Git add mueve los cambios de la carpeta al staging area.

````
    git add nombre_del_archivo
````

### Git commit

Si git add es “preparar”, entonces git commit es “tomar una foto (snapshot)” de esos cambios.Si git add es “preparar”, entonces git commit es “tomar una foto (snapshot)” de esos cambios.

````
    git commit -m "mensaje descriptivo"
````

### Git push

git push sirve para subir tus commits al repositorio remoto.

````
    git push origin nombre_de_la_rama
````

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

## Clase 3
### ¿Que es GitHub?
Es la red social de los programadores, en donde puedes almacenar tus repositorios de manera remota.
### Tipos de clonado
#### Https 
''''
https://github.com/user/repo.git
''''
Usa protocolo web (como navegar en internet)
Te autenticas con:
usuario + token personal (PAT) (ya no contraseña)
VENTAJAS
- Fácil de usar
- No necesitas configuración extra
- Funciona en cualquier red
DESVENTAJAS: 
Tienes que ingresar credenciales (o token) a veces
Menos cómodo para uso frecuente
#### Ssh
''''
git@github.com:user/repo.git
''''
Usa claves criptográficas (una pública y una privada).
Configuras tu llave SSH una vez en tu PC y en GitHub
VENTAJAS:
No tienes que escribir contraseña nunca más
Más seguro y profesional
Ideal para uso constante
DESVENTAJAS: 
Requiere configuración inicial (generar clave SSH)
#### Cli
''''
gh repo clone user/repo
''''
Aquí hay una pequeña confusión: no es un protocolo como HTTPS o SSH, sino una herramienta.
Usas comandos gh
Ya estás autenticado en GitHub CLI
Internamente usa HTTPS o SSH (pero tú no lo notas)
VENTAJAS: 
Más cómodo (no copias URLs)
Integración con GitHub (issues, PRs, etc.)
Ideal para productividad
DESVENTAJAS:
Necesitas instalar la herramienta gh
