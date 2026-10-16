# CPPMD Construction Project Monitoring System (Stages 1 to 3)

React (Vite) + Supabase (PostgreSQL, Auth, Storage).

## Set up
1. Create a project at supabase.com.
2. Open SQL Editor, paste and run `supabase/schema.sql`.
3. Authentication > Users: add your users. Then make the first one admin:
   `update profiles set role='admin' where id='<user uuid>';` Roles: admin, officer, inspector, viewer.
4. `cp .env.example .env` and fill in the project URL and anon key (Project Settings > API).
5. `npm install` then `npm run dev`. For deployment: `npm run build` and host the `dist` folder (Netlify, Vercel, etc.).

## Done in this delivery
Branding and home page, login with roles, database with row-level security, audit log triggers, project register with search and filters, add/edit with validation, full-page project profile, automatic date and money calculations, revised completion history, IPCs, milestones.

## Not yet built (later stages)
Reports with Word/Excel/PDF export, gallery and photo upload (storage bucket and tables already in the schema), analytics charts, alerts, administration screens, backups, automated tests.
All records you add are marked demonstration data until you untick that box.
