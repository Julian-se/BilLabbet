# BilLabbet

A small static site in Swedish. Three pages: start, about, and the first subject (engines). No backend, no database.

## Preview locally

From this folder:

```bash
python3 -m http.server 8080
```

Open http://localhost:8080 and click through Start, Om, and Motor.

## What is live

Production is the `master` branch, hosted on Vercel. The `*.vercel.app` address is already a production environment. A custom domain, once DNS points at the same project, serves that same deployment over HTTPS.

## Update the live site

1. Edit the HTML or CSS.
2. Commit.
3. Push to `master`.

Vercel deploys that push and replaces the files that are public. You do not upload files by hand.

## Domain and HTTPS

Buy the domain at a registrar. In the Vercel project, add the domain. At the registrar, set the DNS records Vercel shows for the apex name and for `www`. When those records resolve, Vercel requests the certificate. You do not install one yourself.
