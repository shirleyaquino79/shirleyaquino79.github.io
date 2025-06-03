## Guardar Proyecto en Github
- cd ruta/a/tu/proyecto
- cd Documentos/mi-proyecto
- git init
- git add .
- git commit -m "Primer commit"
- git remote add origin https://github.com/usuario/nombre-repositorio.git
- git push -u origin master
- git push -u origin main

## Actualizar cambios en Github
- git status 
- git add .
- git commit -m "Descripción de los cambios"
- git push
- git push -u origin main (si es la primera vez o cambiaste rama)

## Cargar Archivos de dos cuentas diferentes
### Usuario A
- git config --global user.name "juan123"
- git config --global user.email "juan123@gmail.com"

### Usuario B

- git config user.name "ana456"
- git config user.email "ana456@gmail.com"

### Cambiar usuario global
- git config --global user.name "OtroNombre"
- git config --global user.email "otro@email.com"

### Verificar usuarios locales
- git config --global user.name
- git config --global user.email
- git config --list --local

## Problemas de Usuarios
remote: Permission to DispositivosHome/prueba3105.git denied to JavierPaniagua.
fatal: unable to access 'https://github.com/DispositivosHome/prueba3105.git/': The requested URL returned error: 403

### Pasos Configuracion Global
1.  
    git config --global user.name
    git config --global user.email

2. git remote set-url origin https://<nuevo-usuario>@github.com/DispositivosHome/prueba3105.git

3. 
    git push origin main

