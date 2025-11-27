# Proyectofinal
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

  Añadir capturas: swagger_ui.png, h2_console.png, logs.png

- 1. Estructura recomendada del repo:
- /backend -> código Java/Spring Boot
- /docs -> postman_collection.json, defense_guide.md, evidences
- /evidence -> screenshots (swagger, h2-console, logs)
- README.md en la raíz

2. GitHub
- Crear repo: parking-backend
- Subir código con gitflow:
  - main (release)
  - develop
  - feature/{feature-name}
- Hacer PR desde feature a develop y desde develop a main (release)

3. Archivos a incluir en la entrega:
- enlace al repo
- capturas en /evidence
- instrucciones de ejecución en README.md
- un pequeño video o GIF (opcional) demostrando la reserva

4. Comandos útiles:
- mvn clean package
- mvn spring-boot:run
- mvn test

  
