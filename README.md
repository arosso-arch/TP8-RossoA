# tp8rossoa

API REST para gestionar un inventario de productos (Trabajo Práctico N° 8).

Spring Boot 3.5 · Java 21 · Spring Web · Spring Data JPA · H2 · Flyway · Lombok

## Cómo ejecutarlo

1. Clonar el repositorio.
2. Copiar `.env.example` como `.env` en la raíz del proyecto y completar los valores.
3. Ejecutar `Tp8rossoaApplication` desde el IDE o con `mvn spring-boot:run`.

La API queda en `http://localhost:8080/productos` y la consola H2 en
`http://localhost:8080/h2-console` (usar la URL, usuario y contraseña del `.env`).

## Endpoints

| Método | Ruta | Éxito | Error |
|---|---|---|---|
| POST | /productos | 201 | 400 |
| GET | /productos | 200 | — |
| GET | /productos/{id} | 200 | 404 |
| PUT | /productos/{id} | 200 | 404 / 400 |
| DELETE | /productos/{id} | 204 | 404 |
| GET | /productos/buscar?nombre=... | 200 | 404 |

En `postman/` hay una colección con todas las pruebas del punto 7.
