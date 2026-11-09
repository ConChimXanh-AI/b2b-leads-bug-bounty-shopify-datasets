# 🌐 B2B Domain Leads, Bug Bounty Subdomain Recon & Shopify Competitor Intelligence (Live Scrapers & Sample Datasets)

[![Apify Store - B2B Lead & Shopify Auditor](https://img.shields.io/badge/Apify_Store-1._B2B_Lead_%26_Shopify_Auditor-00e676?style=for-the-badge&logo=apify)](https://apify.com/conchimxanh_ai/b2b-lead-shopify-auditor)
[![Apify Store - Subdomain & Bug Bounty Recon](https://img.shields.io/badge/Apify_Store-2._Subdomain_%26_Bug_Bounty_Recon-00e5ff?style=for-the-badge&logo=apify)](https://apify.com/conchimxanh_ai/subdomain-ssl-dns-bug-bounty-recon)
[![Apify Store - Shopify Competitor Price Monitor](https://img.shields.io/badge/Apify_Store-3._Shopify_Price_%26_Inventory_Monitor-ffd54f?style=for-the-badge&logo=apify)](https://apify.com/conchimxanh_ai/shopify-competitor-price-monitor)

Welcome to the official open sample repository and API documentation for the **ConChimXanh Cloud Intelligence Suite** on Apify Store.

Whether you are building **B2B outbound sales pipelines**, running **Bug Bounty / Attack Surface Management (ASM) reconnaissance**, or tracking **Shopify & DTC E-Commerce competitor pricing and out-of-stock bestsellers**, you can run our production cloud Actors on-demand via REST API, Python, Node.js, Make.com, n8n, or Zapier.

---

## 🚀 1. B2B Lead Contact, 70+ Tech Stack, DNS/DMARC, SEO & Shopify Auditor
👉 **Run Live on Apify Store**: [**`conchimxanh_ai/b2b-lead-shopify-auditor`**](https://apify.com/conchimxanh_ai/b2b-lead-shopify-auditor)

- **What it extracts**:
  - Verified decision-maker & support emails (with **built-in Cloudflare `data-cfemail` XOR decoder** and **Zero-Browser React/Vue SPA bundle unpacker**).
  - Normalized phone numbers & 10 social media profile channels (LinkedIn, X, Facebook, Instagram, TikTok, YouTube, GitHub, Pinterest, Threads, Telegram).
  - **70+ Technology & Ad Pixel signatures** (Meta Pixel, TikTok Pixel, Google Tag Manager, GA4, HubSpot, Klaviyo, Shopify, Next.js, Cloudflare).
  - Live **DNS/MX Email Provider, SPF, DMARC & SSL Expiry** audit + **Auto-generated Sales Outreach Pitch**.

| Domain | Lead Score | Verified Emails | Phone | Tech Stack | MX Email Provider | Shopify Catalog |
| :--- | :---: | :--- | :--- | :--- | :--- | :--- |
| `colourpop.com` | **100/100** | `colourpop@colourpop.com`, `legal@colourpop.com` | `(949) 224-1810` | Shopify, Klaviyo, Yotpo, Gorgias, GTM | Google Workspace (SPF + DMARC) | 50+ products, Avg `$24.68` |
| `kyliecosmetics.com` | **100/100** | `customerservice@kyliecosmetics.com` | `+8335459543` | Shopify, Klaviyo, Yotpo, Klarna, GTM | Custom Enterprise SMTP | 50+ products, Avg `$63.63` |
| `haravan.com` | **100/100** | `hi@haravan.com` | `1900636099` | Haravan, GTM, Cloudflare, Bootstrap | Google Workspace (SPF + DMARC) | B2B SaaS Platform |
| `topcv.vn` | **100/100** | `hotro@topcv.vn` | `1900068889` | GA4, GTM, Meta Pixel, TikTok Pixel, LinkedIn | Google Workspace | HR Tech Portal |

📂 **Download Free Sample CSV**: [`samples/01_B2B_Leads_TechStack_Shopify_Sample.csv`](./samples/01_B2B_Leads_TechStack_Shopify_Sample.csv)

---

## 🛡️ 2. Subdomain Finder, SSL/TLS, DNS Takeover & Bug Bounty Attack Surface Recon
👉 **Run Live on Apify Store**: [**`conchimxanh_ai/subdomain-ssl-dns-bug-bounty-recon`**](https://apify.com/conchimxanh_ai/subdomain-ssl-dns-bug-bounty-recon)

- **What it extracts**:
  - **4-Source Subdomain Enumeration**: Certificate Transparency (`crt.sh`), AlienVault OTX Passive DNS, HackerTarget HostSearch, and Live TLS SANs (`subjectaltname`).
  - **Dangling CNAME Subdomain Takeover Detection**: Checks discovered subdomains against 16+ vulnerable cloud providers (GitHub Pages, AWS S3, Heroku, Azure, Vercel, Fastly, Shopify, Pantheon).
  - **SSL/TLS Expiry, HTTP Security Headers (HSTS, CSP, X-Frame-Options, Wildcard CORS) & RFC 9116 `/.well-known/security.txt` Bug Bounty Policy Extractor**.

| Root Domain | Subdomains Discovered | Live DNS Resolved | Security Score | SSL Expiry | RFC 9116 `security.txt` | Bug Bounty Policy |
| :--- | :---: | :---: | :---: | :---: | :---: | :--- |
| `hackerone.com` | **42** | **14** | **100/100** | `134 days` | ✅ Yes | `https://hackerone.com/security` |
| `haravan.com` | **56** | **20** | **80/100** | `51 days` | ❌ No | Audited |

📂 **Download Free Sample CSV**: [`samples/02_Bug_Bounty_Subdomains_SSL_Recon_Sample.csv`](./samples/02_Bug_Bounty_Subdomains_SSL_Recon_Sample.csv)

---

## 🛍️ 3. Shopify & E-Commerce Competitor Price, SKU, Discount & Inventory Monitor
👉 **Run Live on Apify Store**: [**`conchimxanh_ai/shopify-competitor-price-monitor`**](https://apify.com/conchimxanh_ai/shopify-competitor-price-monitor)

- **What it extracts**:
  - Paginated `/products.json` & `/collections.json` catalog extraction (plus Schema.org `Product` JSON-LD fallback).
  - Variant-level **SKUs, Live Sale Price vs Compare-At Price (`Discount %`), In-Stock Ratio %, Out-of-Stock Bestseller Signals, and Newest Product Launches**.

| Store Domain | Platform | Products Sampled | Avg Price | Price Range | In-Stock Ratio | On-Sale Markdowns |
| :--- | :---: | :---: | :---: | :---: | :---: | :--- |
| `colourpop.com` | Shopify | 35 (35 SKUs) | `$27.71` | `$1.00 – $125.00` | **91%** (3 sold-out bestsellers) | Active |
| `kyliecosmetics.com` | Shopify | 35 (35 SKUs) | `$63.63` | `$18.00 – $275.00` | **80%** (7 sold-out bestsellers) | **9 products on sale** |

📂 **Download Free Sample CSV**: [`samples/03_Ecommerce_Competitor_Price_Sample.csv`](./samples/03_Ecommerce_Competitor_Price_Sample.csv)

---

## ⚡ Quick API Integration (Node.js / Python / cURL)

Run any Actor directly via the Apify API:

```bash
curl -X POST "https://api.apify.com/v2/acts/conchimxanh_ai~b2b-lead-shopify-auditor/run-sync-get-dataset-items?token=YOUR_APIFY_TOKEN" \
  -H "Content-Type: application/json" \
  -d '{"domains": ["colourpop.com", "haravan.com", "topcv.vn"]}'
```
