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

## Definición de Terminado

Una tarea se considera terminada cuando:

- [ ] Cumple los criterios de aceptación.
- [ ] El código compila, cuando corresponde.
- [ ] Las pruebas aplicables son satisfactorias.
- [ ] La documentación está actualizada.
- [ ] No tiene errores críticos conocidos.
- [ ] Un integrante diferente revisó el PR.
- [ ] El PR fue aprobado e integrado a main.
- [ ] El Issue relacionado fue cerrado.

## Reglas de documentación

- Toda modificación debe realizarse en una rama.
- Los cambios deben asociarse a un Issue.
- Ningún documento se modifica directamente en main.
- Cada Pull Request requiere revisión.
- La integración se realiza con Squash and merge.

- Referenciar issues relacionados cuando existan.
- Asegurar que el pipeline de CI esté en verde.

## Reporte de issues

Usa las plantillas disponibles en `.github/ISSUE_TEMPLATE/`.
