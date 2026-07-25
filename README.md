# Compass Wellbeing CIC – website

A redesigned, single-page marketing website for Compass Wellbeing CIC.
Built as one self-contained `index.html` (inline CSS and JS, inline SVG) plus a
folder of optimised photographs, so it can be hosted anywhere – a static host,
GitHub Pages, an S3 bucket, or dropped into an existing CMS.

## Run it

Open `index.html` in a browser, or serve the folder:

```bash
python3 -m http.server 8000   # then visit http://localhost:8000
```

## What's on the page

- **Hero** – strapline "Helping communities thrive and helping systems work better together", with a real community photo and the compass-rose motif.
- **Stats** – 16 boroughs · 3.5m people · 3,000+ VCFSE organisations · £24m+ to the sector since 2021.
- **Who we are** – the "our story" narrative, the ambition, and "what makes us different".
- **How we create impact** – the four strategic priorities, each with its metric and stakeholder quote.
- **Impact 2024/25** – headline figures alongside a delivery photo.
- **What we focus on** – the five focus areas.
- **Our people & communities** – a photo gallery.
- **Recognised & accredited** – Living Wage Leader Award, Good Business Charter, Certified Social Enterprise, ELFT ownership; with the Living Wage Champion Award photos.
- **Where we work** – interactive region selector and stylised map covering all 16 boroughs (13 NCEL boroughs + Bedfordshire + Luton).
- **Convening** – the Power of Small gathering.
- **Our partners** – a filterable directory of all **52 partner organisations** funded through the NCEL CAMHS Provider Collaborative 2025/26 grant scheme, each tagged with its boroughs and funding stream.
- **Contact** – demo form and details.

## Brand system

| Token | Colour |
|-------|--------|
| Purple (primary) | `#7271ae` |
| Pink | `#c74168` |
| Blue | `#00a1d6` |
| Deep purple | `#4f4e78` |

British English throughout; en dashes (–), never em dashes.

## Content sources

Copy and figures are drawn from material supplied by Compass Wellbeing:

- **Strategy 2026–29 four-pager** – story, ambition, four priorities, five focus areas, headline figures.
- **"Partner with Compass" funding one-pager** (an external-facing document) – impact figures, accreditations, the Power of Small description.
- **NCEL CAMHS Provider Collaborative 2025/26 awards summary** – the full partner list and boroughs.

## Things to confirm or add before going live

These are flagged rather than assumed:

1. **Partner logos.** The partner directory currently shows a coloured monogram tile for each organisation. To drop in a real logo, add its file to `assets/` and give that partner a `logo:'assets/xxx.png'` entry in the `PARTNERS` array in `index.html`. (Partner logo image files could not be fetched automatically from this environment because outbound web access is restricted by policy.)
2. **Publishing the partner list.** All 52 funded organisations are named. Grant awards are usually announced publicly, but please confirm this is intended for the public site.
3. **Bedfordshire and Luton localities.** The exact towns/venues can be expanded, or the stylised map replaced with a live map, once confirmed.
4. **Contact form.** It is a front-end demo; wire it to an email service or CRM to go live.
5. **Deliberately excluded** (from internal-only documents, so kept off the public site): the names of the three event sponsors, any sponsorship pricing/tiers, the founder/CEO wellbeing "idea", and the internal delivery-plan narrative (income, leadership transition, risks). Add any of these only if intended for public use.

## Assets

Photographs in `assets/` were supplied by Compass Wellbeing and resized/optimised for web.
