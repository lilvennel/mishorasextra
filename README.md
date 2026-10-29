# Mis horitas

Calculadora de horas extra con sueldo fijo, feriados, horas a favor, descuentos y cuenta en la nube.

## Archivos
- `public/index.html`: la app completa (un solo archivo).
- `wrangler.jsonc`: configuración para publicar en Cloudflare.
- `supabase-horas-extras.sql`: tablas y seguridad de la base de datos (se corre una vez en el SQL Editor de Supabase; sirve para proyectos nuevos y para actualizar uno existente).

## Publicar
1. Correr `supabase-horas-extras.sql` en Supabase (SQL Editor).
2. Subir estos archivos al repositorio, con la carpeta `public` incluida.
3. Cloudflare compila solo con cada cambio que se sube.

No subas nunca la clave `service_role` de Supabase. La clave `anon` que está en el HTML es pública por diseño: los datos los protege el inicio de sesión.
