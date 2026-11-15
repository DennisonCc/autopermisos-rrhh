# Autopermisos RRHH

Sistema para la gestión y automatización de autopermisos del área de Recursos Humanos.

## Stack

- Java 21
- Spring Boot 3.4
- Maven 3.9
- PostgreSQL 16
- Docker / Docker Compose

## Estructura del repositorio

```text
autopermisos-rrhh/
├── .github/            # CI/CD, plantillas de issues, CODEOWNERS
├── docs/               # Documentación por fases del proyecto
├── src/
│   ├── main/           # Código de producción
│   └── test/           # Pruebas automatizadas
├── scripts/db/         # Scripts de base de datos
├── docker-compose.yml
├── Dockerfile
└── pom.xml
```

## Requisitos

- JDK 21
- Maven 3.9+
- Docker y Docker Compose (opcional)

## Ejecución local

```bash
mvn spring-boot:run
```

La aplicación queda disponible en `http://localhost:8080`. La base de datos se configura con las variables de entorno `DB_URL`, `DB_USERNAME` y `DB_PASSWORD`.

## Ejecución con Docker

```bash
docker compose up --build
```

Esto levanta la aplicación y una instancia de PostgreSQL.

## Pruebas

```bash
mvn verify
```

## Endpoints

| Método | Ruta               | Descripción              |
|--------|--------------------|--------------------------|
| GET    | `/api/v1/health`   | Estado del servicio      |
| GET    | `/actuator/health` | Health check de Spring   |

## Documentación

La documentación del proyecto se organiza en `docs/`:

1. [Planificación](docs/01-planificacion/)
2. [Requisitos](docs/02-requisitos/)
3. [Diseño](docs/03-diseno/)
4. [Construcción](docs/04-construccion/)
5. [Pruebas](docs/05-pruebas/)
6. [Despliegue](docs/06-despliegue/)
7. [Mantenimiento](docs/07-mantenimiento/)

## Contribución

Revisa [CONTRIBUTING.md](CONTRIBUTING.md) antes de enviar cambios.

## Licencia

Este proyecto se distribuye bajo la licencia MIT. Consulta [LICENSE](LICENSE).
