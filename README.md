# 📊 Influencer Analytics Dashboard

Dashboard analítico para influencers construido únicamente con **HTML5 semántico** y **Tailwind CSS v4** (sin frameworks JS ni librerías externas).

## 🚀 Demo

Este proyecto despliega un panel de control con métricas clave para la gestión de campañas de marketing de influencers, incluyendo:

- **KPIs Principales**: Comisiones, facturación, conversión global y alcance.
- **Drivers**: Rendimiento por plataforma, funnel de conversión y rendimiento por producto.
- **Detalles Operacionales**: Tabla de campañas, alertas e insights, y top métricas.

## 🛠️ Requisitos

- [Node.js](https://nodejs.org/) (v18 o superior) — necesario para `npx http-server`

## ▶️ Cómo arrancar el proyecto

```bash
# 1. Clona el repositorio
git clone <url-del-repositorio>
cd dv-dashboard-tailwind

# 2. Inicia el servidor local con http-server
npx http-server
```

Esto levantará el servidor en `http://localhost:8080` (por defecto). Abre esa URL en tu navegador para ver el dashboard.

> **Nota**: No se requiere `npm install` ya que Tailwind CSS se carga vía CDN oficial en el `<head>` del documento.

## 📁 Estructura del proyecto

```
dv-dashboard-tailwind/
├── index.html       # Dashboard completo
├── PROMPTS.md       # Guía de prompts para GitHub Copilot
├── .gitignore       # Archivos ignorados por Git
├── learn.json       # Configuración del proyecto 4Geeks
├── server.py        # Servidor Python alternativo
└── README.md        # Este archivo
```

## 🧩 Tecnologías

- **HTML5** semántico y accesible (SEO & GEO friendly)
- **Tailwind CSS v4** vía CDN
- **Google Fonts** (Inter)
- Diseño **mobile first** y totalmente responsive

## 👤 Autor

Desarrollado por **Deimian Vásquez**  
[dvasquez@4geeksacademy.com](mailto:dvasquez@4geeksacademy.com)

© 2026 Todos los derechos reservados.