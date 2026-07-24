# Guía de Prompts para GitHub Copilot: Influencer Analytics Dashboard

## Prompt 1: Configuración inicial, Layout y Header

Actúa como un Desarrollador frontend Senior Experto en tailwind CSS v4 y HTML5. 

Restricciones técnicas estrictas: 
- Tecnologías permitidas: Únicamente tailwind y HTML5 semántico
- Prohibido usar frameworks o bibliotecas externas de js o framework
- La carga de tailwind es con el cdn oficial en el head
- No utilices clases obsoletas o urls de tailwind 
- El enfoque del diseño es mobile first


Tarea: 
Crea una estructura HTML base (index.html) para un dashboard analítico de influencer

El archivo debe incluir:
1.- Etiqueta head con el script de cdn de tailwind y la tipografía a usar es sans serif
2.- Un layout general con un fondo gris claro y un min height de pantalla completa
3.- El navbar es responsive con:
    - nombre de la app (Metrics deimian) o haz un logo ficticio
    - perfil del influencer con avatar nombre Wolfgang Amadeus (rol creador de contenido musical)
    - filtro de fechas simulado

Genera únicamente la estructura HTML completa descrita.


## Prompt 2

Continuando con la estructura HTML previa, maqueta la primera sección dentro del `<main>`: el "Bloque Superior: KPIs Principales".

CONTEXTO DEL NEGOCIO:
- Producto A: 50 € | Producto B: 120 € | Producto C: 80 €
- Comisión por venta: 15%

REQUISITOS TÉCNICOS:
- Usa componentes Grid responsive: 1 columna en móvil (`grid-cols-1`), 2 en tablet (`sm:grid-cols-2`), y 4 en escritorio (`lg:grid-cols-4`).
- Utiliza etiquetas HTML semánticas y utilidades de Tailwind CSS v4 (tarjetas con sombras suaves, bordes redondeados `rounded-xl`, bordes `border border-slate-200`, y padding adecuado). 

MÉTRICAS A MOSTRAR (Al menos 4 tarjetas de KPI):
1. Comisiones Totales Generadas (€): Muestra el monto total en euros, un indicador positivo de cambio (+18% vs mes anterior) y subtexto informativo.
2. Revenue / Facturación Total Generada (€): Suma total de ventas generadas para las marcas.
3. Conversión Global (%): Tasa de conversión (Conversiones / Alcance total), ej. 3.4%.
4. Alcance e Impresiones Totales: Número consolidado de impresiones en todas las redes (ej. 450K).

Entrega el código HTML del contenedor `<section id="kpis">` listo para insertar en el proyecto.


## Prompt 3

Maqueta la segunda sección dentro del `<main>`: el "Bloque Intermedio: Drivers".

REQUISITOS TÉCNICOS:
- Mantén la restricción: SOLO HTML5 y Tailwind CSS v4.
- Los gráficos simulados deben hacerse usando HTML/Tailwind puro (usando flexbox, anchuras en porcentaje `w-[60%]`, barras de progreso con `bg-indigo-600`, etc.). No utilices <canvas> ni librerías JS.
- Utiliza una cuadrícula layout: 1 columna en móvil, adaptándose a 2 o 3 columnas en pantallas grandes (`lg:grid-cols-3`).

CONTENIDO REQUERIDO (3 Tarjetas de Drivers):
1. Rendimiento por Plataforma (Instagram, TikTok, YouTube):
   - Muestra cada red social con su icono/nombre, barra de porcentaje de ingresos generados y monto en comisiones.
2. Funnel de Conversión (Embudo de Ventas):
   - Pasos visuales simulados con barras HTML: Impresiones -> Clics -> Leads Clickados -> Compras Finales con sus respectivas tasas de conversión por etapa.
3. Rendimiento por Producto (Producto A - 50€, Producto B - 120€, Producto C - 80€):
   - Muestra ventas unidades, comisiones generadas (15%) y tasa de conversión individual de cada producto.

Entrega la sección HTML `<section id="drivers">` estructurada y comentada.


## Prompt 4
Maqueta la última sección dentro del `<main>`: el "Bloque Inferior: Detalles Operacionales y Alertas".

REQUISITOS TÉCNICOS:
- Mantén la regla de SOLO HTML y Tailwind CSS v4.
- Las tablas deben ser completamente adaptativas: usa scroll horizontal (`overflow-x-auto`) para pantallas móviles pequeñas para asegurar la usabilidad.

CONTENIDO REQUERIDO:
1. Tabla de Campañas / Publicaciones Recientes:
   - Columnas: Red Social, Producto Promocionado, Alcance, Clics, Conversiones, Comisiones Generadas (€), Estado (Activa / Finalizada).
   - Diseña las filas con estados de hover (`hover:bg-slate-50`) y badges de colores usando Tailwind (`bg-green-100 text-green-800`).
2. Panel de Alertas e Insight de Rendimiento:
   - Lista de tarjetas pequeñas o mensajes de alerta con bordes laterales de color (`border-l-4`):
     * Pico de conversión: "TikTok superó el CTR promedio en +5% con el Producto B".
     * Caída / Oportunidad: "Instagram Stories requiere optimización de enlace".
3. Listado de "Top Métricas":
   - Badge o lista corta con la "Mejor Plataforma por ROI" y "Producto Más Rentable".

Genera el código HTML completo para `<section id="operacional">` junto con el cierre del archivo HTML.



Recuerda debe ser accesible a SEO y GEO, el dominio es deimianvasquez.com