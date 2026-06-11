# RISE Women's Health Collaborative — Website

Static marketing site for RISE Women's Health Collaborative (evidence-based menopause care, Bozeman MT).

## Structure

```
website/
├── index.html              # Full single-page site (responsive, no build step)
├── images/
│   └── hero-patient.webp   # Hero photo (left-edge alpha feathered to blend into sage bg)
└── README.md
```

## Deploy to GitHub Pages

```bash
# From your local clone of https://github.com/AIrisu88i/website
cp -r /path/to/downloaded/files/* .
git add .
git commit -m "Add RISE website"
git push origin main
```

Then in the GitHub repo:
1. **Settings → Pages**
2. Source: **Deploy from a branch**
3. Branch: **main** / folder: **/ (root)**
4. Save — the site will be live at `https://airisu88i.github.io/website/` within a few minutes

## Before going live (important)

- **Booking form**: The form in `#book` is a visual demo only. Replace it with a HIPAA-compliant embed (Acuity Scheduling with a signed BAA, Jane App, or your EHR's widget). Never collect patient health information through a plain HTML form on GitHub Pages — GitHub Pages is not HIPAA-compliant hosting for PHI.
- **Contact info**: Update placeholder phone/email/address in the footer.
- **Photos**: Replace practitioner placeholder blocks with real photos.
- **Legal pages**: The footer links to Privacy Policy / Notice of Privacy Practices / Medical Disclaimer are placeholders — these pages must exist before launch for a medical practice.
- **Custom domain**: Settings → Pages → Custom domain (e.g., risehealthco.com), then add the CNAME/A records at your registrar.

## Brand tokens

| Token | Hex |
|---|---|
| Sage | `#A3A793` |
| Cream | `#F6F2ED` |
| Terracotta | `#BB6B5A` |
| Charcoal | `#6F695F` |
| Forest | `#3E463E` |

Typography: Cormorant Garamond (serif display) + DM Sans (sans body), loaded from Google Fonts.
