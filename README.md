# Proyecto final
# Parking Backend (Java + Spring Boot + H2)

## Resumen
Backend for the Parking system implemented with Spring Boot (Java) and H2 in-memory database.
Provides REST endpoints for places and reservations and includes OpenAPI UI (Swagger).

## Estructura
- src/main/java/edu.university.parking - código fuente
- src/main/resources/application.properties - configuración (H2)
- pom.xml - Maven build

## Requisitos
- Java 11+
- Maven

## Ejecutar localmente
1. `mvn clean package`
2. `mvn spring-boot:run`
3. API docs: `http://localhost:8080/swagger-ui.html` or `http://localhost:8080/swagger-ui/index.html`
4. H2 console: `http://localhost:8080/h2-console` (jdbc url: jdbc:h2:mem:parkingdb, user: sa)

## Endpoints principales
- GET /api/places
- GET /api/places/<built-in function id>
- POST /api/places
- GET /api/reservations
- GET /api/reservations/<built-in function id>
- POST /api/reservations?plate=ABC123&placeId=1
- POST /api/reservations/<built-in function id>/finish

## Evidencias sugeridas para la entrega
- Capturas del Swagger UI mostrando endpoints.
- Captura del H2 console con tablas.
- Logs del arranque y peticiones.
- Archivo README.md en el repo.
  
Defensa oral

1. Introducción 
- Nombre del proyecto: Parking Backend
- Tecnologías: Java, Spring Boot, H2, Maven, OpenAPI (Swagger)

2. Objetivo 
- Breve: gestionar plazas y reservas, demostrar arquitectura en capas y consumo por frontend.

3. Arquitectura 
- Explicar capas: controllers, services, repositories, model.
- Mostrar diagrama rápido (puede ser un slide): flujo de una reserva.

4. Demostración técnica 
- Levantar la aplicación `mvn spring-boot:run`.
- Mostrar Swagger UI con endpoints.
- Ejecutar: POST /api/reservations?plate=ABC123&placeId=1
- Mostrar que place cambia a occupied=true y que reservation aparece.
- Mostrar H2 console con tablas.

5. Pruebas y evidencia 
- Tests básicos 
- Capturas en /docs o /evidence.

 # Parking Frontend - Template Repo

This repo contains the React frontend for the Parking system.

Run:
- npm install
- npm run dev

  FRONTEND
  Este frontend utiliza Vite y proxy.
  # Parking Frontend (React + Vite)

## Resumen
Frontend minimal para el sistema Parking. Consume el backend en http://localhost:8080 mediante proxy configurado en vite.config.js.

## Requisitos
- Node.js 16+
- npm o yarn

## Instalar y ejecutar
1. `npm install`
2. `npm run dev` (inicia en http://localhost:3000)

## Notas
- El proxy en vite.config.js enruta /api -> http://localhost:8080
- Asegúrate de tener el backend (Java Spring Boot) corriendo en localhost:8080
- Capturas de evidencia en /evidence

- 



  
