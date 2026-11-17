# 🦃 Thanksgiving × Julebord 🇳🇴

A one-page sign-up site for our Eidsvoll melting-pot feast: friends add the dish they're
bringing (🇺🇸 Thanksgiving, 🇳🇴 julebord, or 🌍 family recipe) and it lands on a drawing
of the dinner table. The sidebar suggests what's still missing from both traditions
and shows how balanced the melting pot is.

## Customize
Edit the `EVENT` block at the top of `index.html` (title, date, place).
Edit `NEEDS` / `CATEGORIES` further down to change what counts as "needed".

## Data
Signups live in the `thanksgiving_dishes` table of the **Wanderlings** Supabase project.
The key in `index.html` is the *publishable* key, which is meant to be public.
Row-level security only lets visitors read, add, and remove rows in that one table.

To clear the table after the holiday, run this in the Supabase SQL editor:
```sql
delete from public.thanksgiving_dishes;
```

## Hosting (GitHub Pages)
Repo → Settings → Pages → Source: *Deploy from a branch* → `main` / `(root)`.
