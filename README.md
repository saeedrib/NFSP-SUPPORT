# NFSP SUPPORT

Responsive static application portal for Vercel, connected to the existing Supabase project.

## Important positioning
This is an independent initiative and is not affiliated with nfsp.ng or the Federal Government of Nigeria. ₦70,000 is a proposed support amount only; no selection or payment is guaranteed. Do not collect fees, NIN, BVN, bank credentials, card details, PINs, passwords or OTPs through this form.

## Deploy to Vercel
1. Import `saeedrib/NFSP-SUPPORT` into Vercel.
2. Framework preset: Other.
3. Build command: leave empty.
4. Output directory: `.`.
5. Deploy. The root `index.html` is the site entry point.

The browser uses a Supabase publishable key, which is intended for public clients. Never add a Supabase service-role/secret key to this repository.

## Database
The `nfsp_applications` table is in the Student Loan Found Supabase project. Public users can INSERT only. Public SELECT/UPDATE/DELETE are not granted. An authenticated, role-protected admin workflow must be implemented separately before administrators can view or manage applications.

## Reference codes
A reference code is generated on the client and stored with the application; the same code is shown to the applicant after a successful insert.
