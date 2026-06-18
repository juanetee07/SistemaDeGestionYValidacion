# Sistema de Gestión y Validación de Información Académica

<p align="center">
  Plataforma web para gestionar información institucional y académica dentro de una institución educativa.
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Estado-En%20Desarrollo-orange">
  <img src="https://img.shields.io/badge/Backend-Spring%20Boot-brightgreen">
  <img src="https://img.shields.io/badge/Java-17-orange">
  <img src="https://img.shields.io/badge/Database-MySQL-blue">
</p>

---

## Descripción General

El Sistema de Gestión y Validación de Información Académica tiene como objetivo centralizar la administración de información institucional mediante una plataforma web segura y organizada.

La aplicación permite gestionar:

* Noticias institucionales.
* Resoluciones académicas.
* Usuarios y roles.
* Comentarios y participación de usuarios.
* Control de acceso y permisos.
* Historial y trazabilidad de cambios.

Su propósito es mejorar la comunicación institucional, facilitar el acceso a la información oficial y garantizar la transparencia en la gestión académica.

---

## Objetivos

* Centralizar la información institucional.
* Mejorar el acceso a resoluciones académicas.
* Facilitar la publicación de noticias.
* Garantizar seguridad mediante roles y permisos.
* Mantener un historial de cambios para auditoría.
* Promover la participación de la comunidad educativa.

---

## Módulos del Sistema

| Módulo                  | Descripción                                        |
| ----------------------- | -------------------------------------------------- |
| Inicio                  | Información institucional y acceso general         |
| Noticias                | Publicación y gestión de noticias                  |
| Resoluciones Académicas | Creación, aprobación y publicación de resoluciones |
| Usuarios                | Administración de usuarios                         |
| Roles y Permisos        | Control de acceso según perfil                     |
| Comentarios             | Interacción de usuarios                            |
| Auditoría               | Registro de acciones realizadas                    |

---

## Módulo de Resoluciones Académicas

Este módulo permite gestionar el ciclo completo de vida de una resolución institucional.

### Funcionalidades

* Crear resoluciones.
* Editar resoluciones.
* Aprobar resoluciones.
* Publicar resoluciones.
* Archivar resoluciones.
* Adjuntar documentos PDF.
* Gestionar categorías y etiquetas.
* Consultar historial de cambios.
* Restaurar versiones anteriores.
* Buscar resoluciones mediante filtros.

### Reglas de Negocio

* Una resolución no puede publicarse sin aprobación.
* Solo autoridades autorizadas pueden aprobar resoluciones.
* Las resoluciones no se eliminan físicamente.
* Toda modificación queda registrada en el historial.
* Toda resolución posee autor y fecha de creación.
* Los usuarios solo acceden a información permitida según su rol.

---

## Arquitectura

La aplicación implementa una arquitectura en capas basada en Spring Boot.

```text
Frontend
    ↓
Controllers
    ↓
Services
    ↓
Repositories (JPA)
    ↓
MySQL
```

### Capas

* Controller → Exposición de endpoints REST.
* Service → Reglas de negocio.
* Repository → Acceso a datos.
* Entity → Modelo de dominio.
* DTO → Transferencia de información.
* Security → Autenticación y autorización.

---

## Tecnologías

| Tecnología      | Versión        |
| --------------- | -------------- |
| Java            | 17             |
| Spring Boot     | 3.5.14         |
| Maven           | Última estable |
| MySQL           | 8+             |
| Spring Data JPA | Incluido       |
| Lombok          | Incluido       |
| Validation      | Incluido       |
| DevTools        | Incluido       |

---

## Modelo de Datos

El sistema utiliza un modelo relacional que contempla:

* Usuarios
* Roles
* Noticias
* Resoluciones
* Categorías
* Etiquetas
* Comentarios
* Historial de cambios
* Archivos adjuntos

---

## Metodología de Trabajo

Se utiliza Git Flow para la organización del desarrollo.

### Ramas

```text
main
│
└── develop
      ├── feature/resoluciones
      ├── feature/noticias
      ├── feature/usuarios
      └── feature/comentarios
```

### Flujo de trabajo

* Desarrollo en ramas feature.
* Pull Request hacia develop.
* Validación y pruebas.
* Integración final en main.

---

## Integrantes

* Mayra Yazmín Moyano
* Juan Cruz Larcher
* Tiago Nicolitsis 

---

## Repositorios

### Backend

Backend desarrollado con Spring Boot.

### Frontend

Frontend desarrollado con React.

---

## Estado del Proyecto

🚧 Proyecto actualmente en desarrollo.

### Funcionalidades implementadas

* Estructura base del proyecto.
* Persistencia con JPA.
* Gestión de usuarios.
* Gestión de noticias.
* Gestión de resoluciones académicas.

### Próximas funcionalidades

* Autenticación JWT.
* Auditoría avanzada.
* Historial de versiones.
* Notificaciones.
* Métricas e indicadores.
* Dashboard administrativo.

