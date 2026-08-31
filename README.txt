BARNSLEY FOODBANK PARTNERSHIP — LIVE WAREHOUSE APPLICATION
===========================================================

This package is the first connected web application build.

WHAT IS CONNECTED
-----------------
- Supabase Authentication login
- Supabase PostgreSQL data
- Profiles / roles
- Current stock view
- Stock In
- Stock Out
- Items
- Donors / recipients
- Delivery notes
- Audit / movements
- Branded printable delivery notes
- Responsive layout for warehouse PCs/tablets

IMPORTANT SECURITY
------------------
The application contains the Supabase PUBLISHABLE key. Supabase documents
publishable keys as safe to expose in browser applications when RLS is enabled.
Never put a secret/service_role key in this package.

BEFORE FIRST USE
----------------
1. In your Supabase SQL Editor, run:
   security_policies.sql
2. Make sure your administrator profile exists (you already created it).
3. Create additional staff accounts in Supabase Authentication.
4. Add each new user's profile row with their UUID and role.
5. Open index.html through a web server (not file://) for normal browser use.

TESTING
-------
Start a local web server from this folder, for example:
  python -m http.server 8080

Then browse to:
  http://localhost:8080

DEPLOYMENT
----------
This static app can be deployed to a normal web host. The Supabase URL and
publishable key are in config.js. For production, use HTTPS and a charity-owned
domain/subdomain.

ADDRESS / BRANDING
------------------
Barnsley Foodbank Partnership
Unit 19, Grange Lane Industrial Estate
Carrwood Road, Stairfoot
Barnsley, South Yorkshire, S71 5AS
