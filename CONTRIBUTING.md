# Guía de contribución

Gracias por tu interés en contribuir a Autopermisos RRHH.

## Flujo de trabajo

1. Crea una rama a partir de `main`:

   ```bash
   git switch -c feat/nombre-corto
   ```

2. Realiza los cambios y agrega pruebas cuando aplique.
3. Verifica que el proyecto compile y pase las pruebas:

   ```bash
   mvn verify
   ```

4. Envía un Pull Request describiendo el cambio y su motivación.

## Convención de commits

Se recomienda seguir [Conventional Commits](https://www.conventionalcommits.org/):

- `feat:` nueva funcionalidad
- `fix:` corrección de errores
- `docs:` cambios en documentación
- `refactor:` cambios internos sin alterar comportamiento
- `test:` pruebas
- `chore:` tareas de mantenimiento

## Estilo de código

- Java 21 y las convenciones estándar de Java.
- Formato definido en `.editorconfig`.
- Mantener la arquitectura en capas (`controller`, `service`, `repository`, `domain`, `dto`).
- No incluir credenciales ni secretos en el repositorio.

## Pull Requests

- Un PR por tema.
- Descripción clara del problema y la solución.
- Referenciar issues relacionados cuando existan.
- Asegurar que el pipeline de CI esté en verde.

## Reporte de issues

Usa las plantillas disponibles en `.github/ISSUE_TEMPLATE/`.
