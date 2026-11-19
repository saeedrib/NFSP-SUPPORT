# NFSP SUPPORT

Responsive registration website with a Supabase database and a protected administrator dashboard.

## Deploy to Vercel
1. Import `saeedrib/NFSP-SUPPORT` into Vercel.
2. Framework preset: **Other**.
3. Build command: leave empty.
4. Output directory: `.`.
5. Deploy. The root `index.html` is the applicant registration page.
6. The admin dashboard is available at `/admin.html`.

## Supabase
- The site uses the Supabase publishable key in the browser. Never put a service-role or secret key in this repository.
- Applications are stored in `public.nfsp_applications`.
- Anonymous visitors can submit applications only; they cannot read or update applicant records.
- Authenticated users can read/update applications only if their account has the `admin` role in `public.user_roles`.
- The two existing admin-role accounts in the connected Supabase project can use the admin dashboard with their existing Supabase Auth email and password.
- The form collects NIN and bank account details, so access is restricted to admins. Do not share admin credentials or applicant records.

## Applicant form
The form displays the stated support amount of ₦70,000. Submitting an application does not guarantee selection or payment. Registration is free. BVN, card details, PIN, password and OTP are not requested.

## Admin dashboard
Administrators can review applications, search/filter records, and change individual or bulk application statuses (Pending, Under Review, Approved, Rejected). Sign out after use.
