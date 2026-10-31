# Web Profit Labs

The website is a static HTML export from Framer. There is no build step or package installation required; `index.html` is the homepage.

## Local preview

Serve this folder with any static file server. Root-relative navigation expects the site to be served from a domain root.

## URLs and SEO

The site remains a single page. Navigation links use section URLs such as `/#projects` and `/#services`; these are sections of the homepage, not separate pages.

The canonical URL, sitemap, and GitHub Pages custom domain are configured for `https://webprofitlabs.in/`. Update them if the production domain changes.

## GitHub Pages

The workflow in `.github/workflows/pages.yml` publishes the website files on pushes to `main`. In the repository settings, set **Pages → Build and deployment → Source** to **GitHub Actions**.

The `CNAME` file requests `webprofitlabs.in` as the custom domain. Configure the domain's DNS for GitHub Pages and enable HTTPS in the repository settings before expecting the custom domain to resolve.

The page's images, fonts, and Framer runtime are loaded from Framer's CDN.
