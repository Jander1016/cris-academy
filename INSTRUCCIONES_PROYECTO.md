# 🛠️ PASO A PASO DETALLADO DEL PROYECTO

## PASO 1: Preparación de Terminal
Ejecuta estos comandos en orden para preparar el terreno:
1. `pnpm create astro@latest . -- --template minimal`
2. `pnpm install`
3. `pnpm astro add node tailwind`
4. `pnpm add @clerk/astro @supabase/supabase-js lucide-react`

## PASO 2: El "God Prompt" Inicial
Copia esto en el chat de tu editor una vez creados los .md:

"Hola Gemini. Tengo instalados los archivos MASTER_PLAN.md y ANTIGRAVITY_PROMPTS.md en la raíz. Léelos. 
Tarea inicial: Genera la estructura del Sprint 1: 
- src/styles/global.css (Tailwind)
- src/layouts/MainLayout.astro (Mobile-first)
- src/components/Hero.astro (Minimalista, copy del plan)
- src/pages/index.astro"

## PASO 3: Configuración Externa
1. **Stripe:** Crea el producto y copia el Payment Link en index.astro.
2. **Clerk:** Crea el proyecto y añade las API Keys al archivo .env.
3. **Supabase:** Crea la tabla 'profiles' según el esquema del Master Plan.

## PASO 4: Despliegue en Hostinger
1. Ejecuta `pnpm build`.
2. Sube la carpeta al apartado Node.js de Hostinger.
3. Configura las variables de entorno (Keys de Clerk y Supabase) en el panel de Hostinger.