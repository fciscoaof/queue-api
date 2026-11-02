# Queue API — Bitácora de aprendizaje

Guía de sesiones para aprender Laravel construyendo una API de turnos (*queue management*).
Cada sesión dura **30 min** (10 min de lectura + 20 min de práctica), de lunes a viernes.

## Reglas del juego

1. Cada sesión empieza contigo: abre el archivo de la sesión y escríbele a Claude "Sesión N".
2. Claude te da el objetivo, qué leer, el reto y cómo saber que lo lograste. **No escribe tu código.**
3. Si te trabas, pide pistas: **Pista 1** (concepto o dónde buscar) → **Pista 2** (qué clase o método) → solución solo si la pides después de intentarlo.
4. Revisión: pegas tu código y Claude te señala problemas o te hace preguntas.
5. Cierre: preguntas de comprensión, commit + push y nota en la bitácora de Trello.

## Plan (3 semanas)

| Semana | Objetivo | Temas |
|---|---|---|
| 1 | Base | Instalación y rutas · migraciones y modelos · relaciones Service → Ticket · seeders/factories · CRUD de servicios |
| 2 | Lógica de turnos | Form Requests · `callNext` con transacción · API Resources · manejo de errores · Sanctum |
| 3 | Demostrable | Tests con Pest · README en inglés · GitHub · explicar el proyecto en inglés |
| Después | Docker | Imagen y contenedor · `Dockerfile` · `docker-compose.yml` con PostgreSQL (migración desde SQLite) |

**Base de datos:** SQLite durante el aprendizaje; PostgreSQL al llegar a Docker.

## Vocabulario del dominio

| Español | Código |
|---|---|
| Turno | `Ticket` |
| Servicio | `Service` |
| Llamar el siguiente | `callNext` |
| Finalizar | `complete` |

> Evita llamar un modelo `Queue`: Laravel ya usa *Queues* para trabajos en segundo plano.

## Sesiones

| # | Fecha | Tema | Estado |
|---|---|---|---|
| 01 | 2026-11-02 | [El proyecto andando](session-01.md) | En curso |
