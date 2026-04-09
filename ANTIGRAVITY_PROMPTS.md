# 🚀 GUÍA DE PROMPTS PARA ANTIGRAVITY

## Prompt A: Generación de UI (Frontend)
"Actúa como Senior Frontend Engineer. Basado en MASTER_PLAN.md, genera el componente [NOMBRE] en Astro. Usa Tailwind Mobile-first. Estética minimalista académica. Touch-targets min 44px."

## Prompt B: Lógica de Backend (Supabase/Auth)
"Actúa como Senior Backend Developer. Implementa la conexión con Supabase en src/lib/supabaseClient.ts para manejar el perfil del usuario. Usa los tipos definidos en el Master Plan."

## Prompt C: Seguridad (Middleware)
"Actúa como Software Architect. Configura src/middleware.ts con Clerk para proteger las rutas /campus/*. Si no está logueado o no ha pagado (is_enrolled: false), redirige según corresponda."

## Prompt D: Automatización (Stripe Webhook)
"Actúa como Lead Fullstack. Crea el endpoint src/pages/api/stripe.ts. Al recibir checkout.session.completed, actualiza is_enrolled en Supabase y envía log de confirmación."