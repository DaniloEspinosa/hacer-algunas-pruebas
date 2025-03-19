## HACER ALGUNAS PRUEBAS

La idea de este repositorio es hacer un repaso general de markdown y ramas en git y github

### Pasos a seguir en un nuevo proyecto

- Crear el proyecto
- No olvidar de hacer el archivo .gitignore
- Hacer el archivo README.md para dar las indicaciones necesarias del proyecto
- Crear el repositorio de github
- Inicializar proyecto en git:
    - git init
    - git add .
    - git commit -m "first commit"
    - git branch -M main
    - git remote add origin https://github.com/DaniloEspinosa/hacer-algunas-pruebas.git
    - git push -u origin main
- Crear una rama developer para no afectar la rama de produccion en este caso la main
    - git checkout -b developer
- Subir la rama nueva rama al repositorio
    - git push -u origin developer

