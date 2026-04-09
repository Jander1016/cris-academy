# 📘 MASTER PLAN: Tech Interview Mastery & English Accelerator

## 1. VISIÓN DEL PRODUCTO
- **Objetivo:** Landing page de alta conversión + Portal de Alumno (LMS) privado.
- **Nicho:** Ingenieros de Software Senior que buscan roles FAANG o remotos ($150k+).
- **Propuesta de Valor:** "The Science of High-Stakes Communication for Engineers".
- **Estética:** Minimalista, Profesional, Estilo Académico (Higher Ed).
- **Colores:** Fondo: `#FFFFFF` | Texto: `#0F172A` | Acento: `#1E293B`.
- **Estrategia:** Strictly Mobile-First.

## 2. STACK TECNOLÓGICO
- **Framework:** Astro (Modo SSR con `@astrojs/node`).
- **Styling:** Tailwind CSS.
- **Autenticación:** Clerk (SDK oficial para Astro).
- **Base de Datos:** Supabase (PostgreSQL para perfiles y pagos).
- **Pagos:** Stripe (Payment Links + Webhooks).
- **Contenido:** Astro Content Collections (Archivos .mdx).
- **Hosting:** Hostinger Business (Node.js Managed App).

## 3. ARQUITECTURA DE ARCHIVOS
- `/src/components`: UI Reutilizable (Hero, Pricing, etc).
- `/src/content`: Material académico en archivos .mdx.
- `/src/layouts`: MainLayout (Público) y CampusLayout (Privado).
- `/src/lib`: Clientes de API (Supabase).
- `/src/pages`: 
    - `index.astro`: Landing Page.
    - `/api/stripe.ts`: Webhook de automatización.
    - `/campus/`: Dashboard y visor de lecciones.

## 4. ESTRUCTURA DE BASE DE DATOS (Supabase)
- **Tabla `profiles`**:
    - `id`: uuid (PK, coincide con Clerk ID).
    - `email`: text.
    - `is_enrolled`: boolean (default: false).
    - `cohort`: text (A o B).

## 5. INSTRUCCIONES PARA LA IA (Antigravity)
1. Usar siempre enfoque Mobile-first en Tailwind.
2. Código compatible con adaptador de Node.js para Hostinger.
3. Mantener tono profesional y académico en todo el copy.
4. Priorizar componentes de Astro (.astro) sobre React para velocidad.