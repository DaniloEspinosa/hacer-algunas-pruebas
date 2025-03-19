# REPASO MARKDOWN Y RAMAS GIT - GITHUB

La idea de este repositorio es hacer un repaso general de markdown y ramas en git y github

## Pasos a seguir en un nuevo proyecto

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
- Crear una rama developer para no afectar la rama de producción en este caso la main
    - git checkout -b developer
- Subir la rama nueva rama al repositorio
    - git push -u origin developer
- Al realizar algún cambio:
    - git add . (el el nombre del fichero)
    - git commit -m "Descripción del cambio"
    - git push origin developer
- Crear ramas de características o correcciones a partir de developer
    - git checkout -b feature-nueva-funcionalidad developer
    - Una vez realizados los cambios:
        - git add .
        - git commit -m "Implementé la nueva funcionalidad ..."
        - git push origin feature-nueva-funcionalidad
        - Ahora puedes hacer un Pull Request (PR) desde feature-nueva-funcionalidad hacia developer.
- Fusionar developer con main cuando sea estable
    - Una vez que developer tenga los cambios estables y aprobados, puedes fusionarlos con main:
        - git checkout main
        - git merge developer
        - git push origin main

### Resumiendo el flujo de trabajo en Git
-1️⃣ Crear la rama developer si no existe (git checkout -b developer).
-2️⃣ Trabajar en developer, hacer commit y push regularmente.
-3️⃣ Para nuevas funciones, crear ramas desde developer.
-4️⃣ Hacer Pull Request de las ramas de características a developer.
-5️⃣ Cuando developer esté estable, fusionarlo con main.