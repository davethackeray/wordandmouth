---
description: How to manage and deploy the Word And Mouth website
---

# Website Management Workflow

## Quick Commands

// turbo-all

### View site locally
```bash
cd c:\Users\Thack\Documents\_projects\wam\ideas\wam-site
npm run dev
```
Site runs at http://localhost:4321

### Deploy changes
```bash
git add .
git commit -m "Your change description"
git push
```
Changes auto-deploy to https://wordandmouth.com via GitHub Actions (~2 mins)

### Check deployment status
Visit: https://github.com/davethackeray/wordandmouth/actions

---

## Content Locations

| Content Type | Location | Example |
|--------------|----------|---------|
| Case Studies | `src/pages/case-studies/` | `tbt.astro` |
| Insights/Blog | `src/pages/play/` | `blog.astro` |
| Industry Hubs | `src/pages/industries/[industry].astro` | Dynamic routes |
| Static Assets | `public/` | Images, prototypes |
| Prototypes | `public/prototypes/` | `tbt/index.html` |

## Tagging System

See `.agent/content-guide.yaml` for:
- **Tenets**: story, clarity, insight, ai, growth
- **Industries**: saas, agency, media, fintech, ecommerce, professional, health, education

## Common Tasks

### Add a new case study
1. Create `src/pages/case-studies/[name].astro`
2. Copy structure from existing case study
3. Tag with tenets and industry
4. Push to deploy

### Add new insight/blog post
1. Edit content in `src/pages/play/blog.astro`
2. Or create new page in `src/pages/play/`
3. Push to deploy

### Update homepage
1. Edit `src/pages/index.astro`
2. Push to deploy

### Add new prototype
1. Create HTML file in `public/prototypes/[name]/index.html`
2. Reference in case study with iframe
3. Push to deploy
