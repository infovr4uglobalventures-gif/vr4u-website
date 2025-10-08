# VR4U Site - Ready for Netlify

This is a Vite + React + Tailwind project prepared for deployment to Netlify.

## Quick setup (local)
1. Install Node.js (v18+ recommended).
2. Run `npm install`
3. Run `npm run dev` to preview locally.
4. Run `npm run build` to build production files into `/dist`.

## Deploy to Netlify
1. Create a Netlify account and connect your Git repository (GitHub/GitLab/Bitbucket) or drag-and-drop the `dist` folder into Netlify's site deploy area.
2. If connecting repo, set build command to `npm run build` and publish directory to `dist`.
3. After deployment, configure your custom domain (see below).

## Custom Domain Setup (example)
1. Buy a domain through a registrar (GoDaddy, Namecheap, Google Domains, etc.)
2. In Netlify dashboard, go to **Domain settings → Add custom domain** and enter your domain (e.g. `vr4uglobal.com`).
3. Netlify will provide DNS records:
   - Add the provided `A` records and `CNAME` in your registrar's DNS settings.
   - Alternatively, point the domain with the provided `nameservers` (if you want Netlify to manage DNS).
4. Enable HTTPS by turning on the Let's Encrypt certificate in Netlify (Netlify usually provisions it automatically).
5. Allow DNS changes to propagate (can take up to 24-48 hours, often faster).

## Notes
- The contact form in this template is a stub (uses `alert`). To receive messages:
  - Integrate with Netlify Forms (add `data-netlify="true"` to the form and redeploy), or
  - Use a service like Formspree, Getform, or a serverless function / API endpoint.
- Replace placeholder contact info and phone numbers with real details.

