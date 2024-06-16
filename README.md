# Propósito de la Documentación
Esta documentación está diseñada para proporcionar una guía clara y estructurada sobre el uso de Git en proyectos, incluyendo los comandos esenciales para iniciar un repositorio y buenas prácticas para la escritura de mensajes de commit. Siguiendo esta guía, se garantiza un flujo de trabajo ordenado y consistente, facilitando la colaboración y el mantenimiento del código.

# Comandos Esenciales para Iniciar un Proyecto en Git y Vincularlo a GitHub
La sección inicial de comandos proporciona una serie de pasos para configurar un nuevo proyecto Git, agregar archivos, hacer el primer commit, crear la rama principal y vincular el repositorio local a un repositorio remoto en GitHub. Estos comandos son:

# INICIAR EL GIT EN UN PROYECTO VACIO Y VINCULARLO AL GITHUB.

```bash
git init
```

```bash
git add .
```

```bash
git commit -m "Initial commit"
```

```bash
git branch -M main
```

```bash
git remote add origin https://github.com/Julian1699/Mis-Apuntes.git
```

```bash
git push -u origin main
```

# Buenas Prácticas para Hacer Commits

Esta sección describe las convenciones recomendadas para escribir mensajes de commit claros y útiles, siguiendo un formato específico que incluye el tipo de cambio, el alcance y un resumen breve del cambio. Estas prácticas facilitan la comprensión del historial de cambios y la colaboración en el proyecto.

## Formato del Mensaje de Commit

`<tipo>(<alcance>): <resumen>`

### Tipo

Describe la naturaleza del cambio. Ejemplos:

- `feat`: Nueva funcionalidad
- `fix`: Corrección de errores
- `docs`: Cambios en la documentación
- `style`: Cambios que no afectan la lógica del código (espacios en blanco, formateo, etc.)
- `refactor`: Cambios que mejoran el código sin afectar su funcionalidad
- `test`: Añadir o corregir tests
- `chore`: Actualización de tareas de build, cambios en herramientas, etc.

### Alcance (opcional)

Indica la sección del código que se ve afectada.

### Resumen

Descripción breve del cambio (menos de 50 caracteres).

## Uso del Tiempo Verbal Imperativo

Escribe los mensajes como si estuvieras dando una orden. Ejemplo: `Add new login feature` en lugar de `Added new login feature`.

## Ejemplos de Commits

### feat: Añadir una nueva funcionalidad.

```bash
git commit -m "feat(auth): add user login feature"
´´´

### fix: Corregir un error.

´´´bash
git commit -m "fix(auth): handle token expiration correctly"
´´´

### docs: Actualizar la documentación.

´´´bash
git commit -m "docs(readme): update installation instructions"
´´´

### style: Cambios de formato y estilo del código.

´´´bash
git commit -m "style(css): fix spacing issues in header"
´´´

### refactor: Refactorización del código sin cambiar su funcionalidad.

´´´bash
git commit -m "refactor(user-service): optimize user data processing"
´´´

### test: Añadir o modificar pruebas.

´´´bash
git commit -m "test(auth): add tests for login endpoint"
´´´

### chore: Cambios en tareas de mantenimiento.

´´´bash
git commit -m "chore(deps): update dependency versions"
´´´
