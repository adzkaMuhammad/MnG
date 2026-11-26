# Direct — klon Instagram DM (React + Supabase)
1. Supabase: buat project → **SQL Editor** → jalankan `supabase/schema.sql`.
2. Supabase → **Authentication → Providers → Email**: matikan "Confirm email" (agar tim langsung bisa login).
3. Salin `.env.example` → `.env`, isi URL dan anon key (Project Settings → API).
4. Lokal: `npm i && npm run dev`.
5. GitHub: `git init && git add . && git commit -m init && git remote add origin <url> && git push -u origin main`.
6. Vercel: Import repo (preset Vite otomatis) → Environment Variables: `VITE_SUPABASE_URL`, `VITE_SUPABASE_ANON_KEY` → Deploy.
7. Supabase → Authentication → URL Configuration: isi Site URL dengan domain Vercel.

Batas: file maks 50 MB (ubah di bucket `media`). Bucket `media` publik (URL berisi UUID acak, tidak bisa ditebak, tapi siapa pun yang punya URL bisa membuka).
