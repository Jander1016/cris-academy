# 🚀 Cris Academy: TODO Roadmap

## ✅ COMPLETADO HOY
- [x] Configuración inicial (Astro, Tailwind 4, TS Strict).
- [x] Diseño de Landing Page Mobile-First.
- [x] Mejora de imagen y marca personal (Dr. Codina).
- [x] Integración de testimonios dinámicos (YouTube & Shorts).
- [x] Conexión con Stripe Payment Links (Flujo de ventas real).
- [x] Configuración base de i18n (Internacionalización).

## 📅 MAÑANA: FASE 3 & 4 (Autenticación y Datos)
### 1. Sistema Multidioma
- [ ] Crear estructura de carpetas `/src/pages/es/` y `/src/pages/en/`.
- [ ] Implementar `ui.ts` para diccionarios de traducciones.
- [ ] Selector de idioma en el Header.

### 2. Autenticación (Clerk)
- [ ] Configuración de API Keys en `.env`.
- [ ] Creación de páginas `/sign-in` y `/sign-up`.
- [ ] Middleware para proteger el `/campus`.

### 3. Base de Datos (Supabase)
- [ ] Crear tabla `profiles` con RLS (Row Level Security).
- [ ] Sincronizar campo `is_enrolled` para acceso al curso.

## 🎓 PRÓXIMAMENTE: FASE 5 & 6 (LMS & Automatización)
- [ ] **Stripe Webhook:** Automatizar la creación de cuentas tras el pago.
- [ ] **LMS Interface:** Visor de lecciones con Content Collections.
- [ ] **Onboarding:** Email de bienvenida automático.
