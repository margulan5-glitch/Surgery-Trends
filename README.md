# Surgery Trends 2026

Registration website and protected admin panel for СНК «Surgery Trends».

## Setup
1. Create a Supabase project.
2. Run supabase-schema.sql in SQL Editor.
3. Create an administrator in Supabase Authentication.
4. Insert that user's UUID into public.admins:
   insert into public.admins (id,email) values ('AUTH_USER_UUID','admin@example.com');
5. Put the Supabase URL and public anon key into js/config.js.
6. Publish the repository with GitHub Pages.
7. Public registration: index.html
8. Admin panel: admin.html

## Security
Never put the Supabase service_role key in the repository. Only the public anon key belongs in browser code. RLS protects application data. For production, add CAPTCHA/rate limiting, custom domain and backups.

The original surgery_trends_registration_2026.html remains as a reference.