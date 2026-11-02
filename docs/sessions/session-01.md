# Sesión 01 — El proyecto andando

**Fecha:** 2026-11-02 · **Duración:** 30 min · **Semana:** 1 (Base)

## Objetivo

Dejar el proyecto funcionando con SQLite, con un endpoint de prueba respondiendo y el primer commit en GitHub.

## Dónde estás

- ✅ Proyecto creado con el instalador (sin starter kit, con Pest) en `C:\Users\srfra\Herd\queue-api`.
- ✅ Base de datos: **SQLite** (decidido 2026-11-02). PostgreSQL se retoma en el módulo de Docker.
- ⚠️ `APP_NAME` sigue como `Laravel`.
- ⚠️ No existe `routes/api.php` (solo `web.php` y `console.php`).
- ✅ Primer commit subido a GitHub (`fciscoaof/queue-api`).

## 1. Lectura (10 min)

En [laravel.com/docs](https://laravel.com/docs):

- **Installation** → sección *Databases & Migrations*.
- **Directory Structure** → fíjate en `app/`, `routes/`, `database/`, `bootstrap/` y `.env`.
- **Routing** → busca *API Routes*.

## 2. Actividades (20 min)

1. **Configura el entorno:** cambia el nombre de la app en `.env` y revisa dónde vive el archivo de SQLite.
2. **Investiga:** ¿qué archivo es tu base de datos y por qué no se sube a git?
3. **Corre las migraciones** iniciales sin errores.
4. **Habilita las rutas de API.** Pista para pensar: hay un comando de `artisan` que lo hace por ti. Descubre cuál y qué archivos modifica.
5. **Crea el endpoint** `GET /api/ping` que responda `{"status": "ok"}`.
6. **Primer commit y push** a un repositorio público en GitHub (mensaje en inglés).

## 3. Checklist

- [ ] `APP_NAME` actualizado en `.env`
- [ ] Ubicado el archivo de base de datos SQLite
- [ ] Migraciones corridas; las tablas por defecto aparecen en la base (TablePlus de Herd, o `php artisan db:show`)
- [ ] Rutas de API habilitadas (`routes/api.php` existe)
- [ ] `GET /api/ping` responde `{"status": "ok"}` (navegador o Postman)
- [ ] Revisado `.gitignore`: `.env` y `vendor/` no se suben
- [x] Primer commit hecho (`Initial laravel project setup`)
- [x] Repositorio en GitHub creado y `push` hecho
- [ ] Commit con `docs/` y el endpoint (ej. `Add ping API endpoint`)
- [ ] Preguntas de cierre respondidas
- [ ] Sesión anotada en la Bitácora diaria (Trello)

## 4. Lo lograste si…

- `http://queue-api.test/api/ping` (Herd) devuelve el JSON esperado.
- Ves las tablas `users`, `cache`, `jobs`, `migrations` en tu base SQLite.
- Tu repo en GitHub muestra el primer commit y **no** contiene `.env`.

## 5. Preguntas de cierre

Respóndelas con tus palabras (aquí abajo o a Claude):

1. ¿Para qué sirve `.env` y por qué no se sube a git?
2. ¿Qué diferencia hay entre `routes/web.php` y `routes/api.php`? ¿Qué prefijo y middleware recibe cada uno?
3. ¿Qué es `artisan` y qué comandos usaste hoy?

**Mis respuestas:**

1.
2.
3.

## 6. Notas

- **Laravel Boost:** el instalador agregó `AGENTS.md`, `CLAUDE.md`, `.mcp.json` y otros archivos para agentes de IA. Mientras aprendes, no le pidas a un agente que escriba el código por ti. Decide si los dejas en el repo o los agregas a `.gitignore`.
- **Docker:** queda para después de terminar la API. No uses Sail por ahora. Ahí migraremos de SQLite a PostgreSQL.

**Dónde me trabé / qué aprendí:**

-
