# Khushal Sehrawat Portfolio

A single-page Java full-stack developer portfolio built with HTML, Bootstrap, JavaScript, GSAP and AOS. The existing portfolio content, project links, branding, title, description and Open Graph metadata are preserved.

## Local preview

Serve this directory with a static web server, for example `python -m http.server 8000`, then open `http://localhost:8000`.

Fonts, styles and libraries are loaded from external services and require an internet connection. No package manifest, configured lint suite or build command is present.

## SEO metadata

Khushal Sehrawat is identified as the portfolio author; TheBenzzCreations is identified as the website creator. Twitter card metadata and an Open Graph site name supplement the existing search and social metadata.

The existing JSON-LD block now contains one graph with the original Person record and a WebSite record. The website references that Person as author and TheBenzzCreations as creator. A visible developer credit appears in the existing footer with a normal same-tab hyperlink for the developer link.

Production identity is recorded in `seo-sites.json`; see Canonical URL validation below. The developer credit is not evidence of a project deployment URL.

## Development & Maintenance

**Developed & Maintained by
[Khushal Sehrawat](https://github.com/khushalsehrawat)**
— Founder of
[TheBenzzCreations](https://www.thebenzzcreations.com/).

TheBenzzCreations is a digital development studio specializing in website development, custom software, mobile applications, e-commerce solutions and AI-powered business automation.

For development enquiries and collaborations, visit [TheBenzzCreations](https://www.thebenzzcreations.com/).

## Canonical URL validation

Run `python scripts/validate_seo.py` from this repository before publishing. The dependency-free check validates exact page canonicals, Open Graph URLs, website/application JSON-LD URLs, sitemap locations, robots sitemap references and literal framework site metadata against `seo-sites.json`. It checks deployment path prefixes as well as domains, so one GitHub Pages project cannot canonicalize to another.

Only URLs whose live HTML matched the local page on 2026-11-21 are configured. Unverified pages have no canonical or social URL; `python scripts/validate_seo.py --require-verified` also fails for those pending pages. Reverify the configuration if the deployment moves. Dynamic framework expressions still require runtime validation.

TheBenzzCreations attribution, creator organization URLs and existing normal same-tab developer credit links are preserved. These outbound attribution links are separate from site identity.
