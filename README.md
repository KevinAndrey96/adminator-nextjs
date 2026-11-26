# Adminator Next.js: panel administrativo con Next.js 13, React y Tailwind

[![Next.js](https://img.shields.io/badge/Next.js-13.5-000000?logo=nextdotjs&logoColor=white)](https://nextjs.org/)
[![React](https://img.shields.io/badge/React-18-61DAFB?logo=react&logoColor=black)](https://react.dev/)
[![TypeScript](https://img.shields.io/badge/TypeScript-5-3178C6?logo=typescript&logoColor=white)](https://www.typescriptlang.org/)
[![Tailwind CSS](https://img.shields.io/badge/Tailwind%20CSS-3-06B6D4?logo=tailwindcss&logoColor=white)](https://tailwindcss.com/)
[![Chart.js](https://img.shields.io/badge/Chart.js-4-FF6384?logo=chartdotjs&logoColor=white)](https://www.chartjs.org/)
[![FullCalendar](https://img.shields.io/badge/FullCalendar-6-2c3e50)](https://fullcalendar.io/)

Panel administrativo (dashboard) construido con Next.js y el App Router, que sigue la estructura de la plantilla Adminator: tarjetas de indicadores, gráficos, calendario, correo, chat, formularios, tablas, mapas y pantallas de acceso.

## Qué problema resuelve

Ofrece una base de interfaz de administración lista para conectar a cualquier API, con las pantallas habituales de un backoffice ya resueltas, para no repetir ese trabajo en cada proyecto.

## Pantallas

| Ruta | Contenido |
| :--- | :--- |
| `/` | Tablero principal con indicadores y gráficos de Chart.js |
| `/calendar` | Calendario con vistas de mes, semana, día y lista |
| `/charts` | Gráficos con Recharts |
| `/chat`, `/email`, `/compose` | Mensajería, bandeja de correo y redacción |
| `/forms`, `/ui` | Formularios y catálogo de componentes de interfaz |
| `/tables/basic`, `/tables/data` | Tablas simples y tablas de datos |
| `/maps/google`, `/maps/vector` | Mapas de Google y mapas vectoriales |
| `/signin`, `/signup` | Inicio de sesión y registro |
| `/blank`, `/404`, `/500` | Página en blanco y páginas de error |

## Estructura

```
.
├── app/
│   ├── layout.tsx            # Layout raíz y tema
│   ├── page.tsx              # Tablero principal
│   ├── components/           # Componentes compartidos (gráficos, layout, tema)
│   ├── hooks/                # Hooks de React
│   └── <ruta>/page.tsx       # Una carpeta por pantalla (calendar, charts, chat...)
├── public/                   # Imágenes y scripts de la plantilla
├── styles/                   # Estilos Sass
├── types/                    # Tipos de TypeScript
├── tailwind.config.ts
└── next.config.js
```

## Requisitos

- Node.js 18 o superior.
- npm, yarn o pnpm.

## Ejecución local

```bash
git clone git@github.com:KevinAndrey96/adminator-nextjs.git
cd adminator-nextjs
npm install
npm run dev
```

Abre `http://localhost:3000`.

Otros comandos: `npm run build` (compilación de producción), `npm run start` (servidor de producción) y `npm run lint`.

## Licencia

Sin licencia de código abierto. Todos los derechos reservados.
