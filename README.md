Ibex Market Map 2
Simple static site with two pages for the Winter 2026 Ibex workflow:

index.html: market map view
sales_funnel.html: deal flow / funnel view
Local development
No build step is required. Open either file directly in your browser, or run a local static server.

Option 1: Open files directly
Open index.html
Open sales_funnel.html
Option 2: Run a local server (recommended)
From the repo folder run:

python3 -m http.server 8000

Then visit:

http://localhost:8000/index.html
http://localhost:8000/sales_funnel.html
Data source
Both pages fetch data from a Google Apps Script endpoint configured in each page’s CONFIG object.

If you need to switch data sources, update endpointBase in:

index.html
sales_funnel.html
Deploy
Because this is static HTML/CSS/JS, it can be deployed to:

GitHub Pages
Netlify
Vercel (static)
Any simple web server
