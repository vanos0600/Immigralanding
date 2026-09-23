🇨🇿 ImmigraSmart — Landing Page
The official static storefront for ImmigraSmart — the AI-powered immigration assistant built for international students navigating the Czech Republic.

📦 Project Structure
Plaintext
immigrasmart-vercel/
├── index.html       # The entire frontend (HTML + CSS + JS in one file)
├── vercel.json      # Vercel configuration (security headers, caching)
├── package.json     # Project metadata
└── README.md        # You are here
Note: Zero build steps required. This is pure, lightweight static HTML — it deploys exactly as is.

🚀 Deployment (3 Ways to Ship It)
Option 1 · Drag & Drop (The Fastest Route)
Compress the immigrasmart-vercel folder into a .zip file.

Head over to vercel.com/new.

Drag and drop the zip file directly onto the dashboard.

Vercel will automatically detect the static setup.

Click Deploy — your site will be live in ~10 seconds.

Option 2 · Via GitHub (Recommended for Production)
Push this folder to a fresh GitHub repository to unlock continuous deployment:

Bash
cd immigrasmart-vercel
git init
git add .
git commit -m "Initial commit"
git branch -M main
git remote add origin https://github.com/YOUR-USERNAME/immigrasmart-landing.git
git push -u origin main
Go to vercel.com/new and link your GitHub account.

Import the immigrasmart-landing repository.

Vercel will detect the package.json. Keep the Framework Preset as Other.

Click Deploy.

Every subsequent git push to main will trigger an automatic deployment. PRs and branches will generate live preview URLs.

Option 3 · Vercel CLI (For Terminal Power Users)
Bash
# Install the CLI (one-time setup)
npm i -g vercel

# Navigate to the project directory
cd immigrasmart-vercel

# Deploy to preview
vercel

# Ship to production
vercel --prod
🌐 Custom Domains
Once deployed, making it officially yours is simple:

Navigate to your project dashboard in Vercel.

Go to Settings → Domains.

Enter your custom domain (e.g., immigrasmart.com).

Vercel will provide the DNS records to add to your registrar (Namecheap, GoDaddy, Cloudflare, etc.).

SSL certificates are generated and renewed automatically for free.

🛠️ Local Development
Want to test tweaks before shipping?

Bash
# Option 1 — Open the file directly
open index.html        # macOS
xdg-open index.html    # Linux
start index.html       # Windows

# Option 2 — Spin up a local server (Recommended)
npx serve .
# or
python3 -m http.server 8000
🎨 Quick Customization
Everything is self-contained in index.html. The core design system is controlled by CSS variables at the top of the <style> block:

CSS
:root{
  --cz-blue: #11457E;     /* Primary Czech Blue */
  --cz-red:  #D7141A;     /* Primary Czech Red */
  --ink:     #0B1B3A;     /* Deep text color */
}
Update these hex codes, and the entire UI will adapt instantly.

Links to Update:
If you change your repository or demo domain, find and replace these URLs in the HTML:

[https://immigrasmart.streamlit.app/](https://immigrasmart.streamlit.app/) → Your live app URL

[https://github.com/vanos0600/ImmigraSmart](https://github.com/vanos0600/ImmigraSmart) → Your GitHub repo

✅ Post-Launch Checklist
[ ] Site loads instantly at your-project.vercel.app

[ ] "Launch the live demo" CTA routes correctly

[ ] "View on GitHub" CTA points to the right repository

[ ] UI remains responsive on mobile devices

[ ] Custom domain successfully mapped (optional)

[ ] Share the link with the world 🚀

👨‍💻 Creators
Oskar David Vanegas Juarez

Ayon Das

📄 License
This project is licensed under the MIT License — feel free to use, modify, and distribute it.

Built with ❤️ in Prague.
