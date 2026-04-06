# GPT Platform

Plataforma web tipo ChatGPT construida sobre infraestructura propia, con soporte para mensajes de texto, audio, imágenes y documentos PDF.

## Demo

> Video de demostración: [próximamente]

## Características

- Chat con IA usando Claude API (Anthropic) y GPT-5
- Entrada por texto, audio e imagen
- Lectura y documentación de archivos PDF
- Backend orquestado con n8n
- Desplegado en VPS propio con Caddy y Cloudflare

## Arquitectura
Usuario → Cloudflare → VPS (Caddy) → n8n → Claude API / OpenAI
↓
Servidor local (PostgreSQL)
## Stack

| Capa | Tecnología |
|---|---|
| Frontend | HTML, CSS, JavaScript |
| Orquestación | n8n |
| IA | Claude API (Anthropic), GPT-5 |
| Base de datos | PostgreSQL |
| Servidor web | Caddy |
| Red | Cloudflare Tunnel |

## Flujos n8n

Los flujos de automatización están en la carpeta `/n8n-flows/` exportados en formato JSON.

## Base de datos

El esquema de la base de datos está en `/database/schema.sql`.

## Autor

Daniel Acevedo — [portfolio.endanus.online](https://portfolio.endanus.online)
