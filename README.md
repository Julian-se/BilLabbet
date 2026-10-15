# BilLabbet

A small static site in Swedish. Pages: Start (`index.html`), Om (`om.html`), Motor (`motor.html`), Service (`service.html`), and Sprängskiss (`sprangskiss.html`). No backend, no database.

## Preview locally

From this folder:

```bash
python3 -m http.server 8080
```

Open http://localhost:8080 and click through Start, Om, Motor, Service, and Sprängskiss.

## What is live

Production is hosted on Vercel: https://billabbet.vercel.app

That address is already a production environment, with HTTPS. A custom domain, once DNS points at the same project, serves that same deployment.

## Update the live site

1. Edit the HTML or CSS.
2. Commit.
3. Push to `master`.

Vercel deploys that push and replaces the files that are public. You do not upload files by hand.

## Domain and HTTPS

Buy the domain at a registrar. In the Vercel project, add the domain. At the registrar, set the DNS records Vercel shows for the apex name and for `www`. When those records resolve, Vercel requests the certificate. You do not install one yourself.
