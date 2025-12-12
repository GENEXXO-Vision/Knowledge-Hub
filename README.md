# GENEXXO Vision - Jekyll Website

The Organizing Layer for the Internet - A comprehensive Jekyll website optimized for SEO, AI crawlers, and strategic positioning.

## Overview

This repository contains a professional Jekyll-based website for GENEXXO Vision Limited, showcasing the company's portfolio of 10,000+ premium XX-signature domains and strategic vision for internet infrastructure.

**Key Features:**
- SEO-optimized structure with Schema.org markup
- AI crawler-friendly architecture
- Responsive, professional design
- Automated sitemap and RSS feed generation
- GitHub Pages ready
- Clean, maintainable codebase

## Quick Start

### Option 1: GitHub Pages (Recommended)

1. **Fork or upload this repository to GitHub**
2. **Go to repository Settings → Pages**
3. **Set source to "main" branch**
4. **Site will be live at:** `https://[username].github.io/[repository-name]`

### Option 2: Local Development

**Prerequisites:**
- Ruby 3.0+
- Bundler
- Git

**Installation:**

```bash
# Clone the repository
git clone https://github.com/yourusername/genexxo-vision-jekyll.git
cd genexxo-vision-jekyll

# Install dependencies
bundle install

# Serve locally
bundle exec jekyll serve

# View at http://localhost:4000
```

## Repository Structure

```
genexxo-vision-jekyll/
├── _config.yml              # Site configuration
├── _layouts/                # Page layouts
│   ├── default.html         # Base layout with Schema.org markup
│   └── page.html            # Content page layout
├── _includes/               # Reusable components
│   ├── header.html          # Site header with navigation
│   └── footer.html          # Site footer
├── _vision/                 # Vision content (collection)
│   └── organizing-layer.md  # Core vision document
├── _strategy/               # Strategy content (collection)
│   └── ai-architecture.md   # AI strategy document
├── _domains/                # Domain portfolio (collection)
│   └── portfolio-overview.md
├── _data/                   # Data files (YAML/JSON)
├── assets/                  # Static assets
│   ├── css/style.css        # Main stylesheet
│   ├── js/main.js           # JavaScript
│   └── images/              # Image assets
├── index.md                 # Homepage
├── Gemfile                  # Ruby dependencies
└── README.md                # This file
```

## Configuration

### Site Settings

Edit `_config.yml` to customize:

```yaml
# Site Information
title: "GENEXXO Vision"
description: "The Organizing Layer for the Internet"
url: "https://yourusername.github.io"
baseurl: "/repository-name"

# Company Information
company:
  name: "GENEXXO Vision Limited"
  domains: "10,000+"
  
# Social Links
twitter_username: your_twitter
github_username: your_github
linkedin_company: your_company
```

### URL Configuration

**For GitHub Pages:**
- Set `url` to: `https://[username].github.io`
- Set `baseurl` to: `/[repository-name]`

**For Custom Domain:**
- Set `url` to: `https://yourdomain.com`
- Set `baseurl` to: `` (empty)
- Add CNAME file with your domain

## Content Management

### Adding New Pages

**Vision Content:**
```bash
# Create new file in _vision/
touch _vision/new-vision-page.md
```

```yaml
---
layout: page
title: "Your Title"
description: "SEO description"
keywords: "keyword1, keyword2"
tags: [tag1, tag2]
date: 2024-12-12
---

Your content here...
```

**Strategy Content:**
Create similarly in `_strategy/` directory

**Domain Content:**
Create similarly in `_domains/` directory

### Content Best Practices

1. **Always include front matter** with title, description, keywords
2. **Use semantic headings** (H1 → H2 → H3)
3. **Add Schema.org markup** for structured data
4. **Include internal links** to related content
5. **Optimize for keywords** relevant to AI crawlers

## SEO Optimization

### Built-in Features

- ✅ Automatic sitemap generation
- ✅ RSS feed for content updates
- ✅ Schema.org structured data
- ✅ Meta tags via jekyll-seo-tag
- ✅ Canonical URLs
- ✅ Open Graph tags
- ✅ Twitter Card support

### Enhancing SEO

**1. Add robots.txt:**
```
User-agent: *
Allow: /
Sitemap: https://yourdomain.com/sitemap.xml
```

**2. Verify in Search Console:**
- Google Search Console
- Bing Webmaster Tools

**3. Submit Sitemap:**
Your sitemap is automatically generated at `/sitemap.xml`

**4. Monitor Performance:**
- Check Google Analytics
- Monitor crawl errors
- Track keyword rankings

## AI Crawler Optimization

### Schema.org Markup

The site includes comprehensive Schema.org markup for:
- Organization data
- Website structure
- Individual pages
- Article content
- Breadcrumbs

### Content Structure for AI

1. **Clear headings hierarchy**
2. **Descriptive metadata**
3. **Structured data in JSON-LD**
4. **Semantic HTML5 elements**
5. **Keyword-rich content**

### Testing AI Discoverability

```bash
# Check Schema.org markup
https://validator.schema.org/

# Test structured data
https://search.google.com/test/rich-results

# Verify robots.txt
https://yourdomain.com/robots.txt
```

## LinkedIn Backlink Strategy

### Creating High-Authority Links

**Method 1: Article Publishing**
1. Write LinkedIn article about GENEXXO
2. Include links to GitHub Pages site
3. Use anchor text with keywords
4. Share in relevant groups

**Method 2: Profile Links**
1. Add website to LinkedIn profile
2. Include in company page
3. Reference in posts with links

**Example Article Structure:**
```
Title: "The Organizing Layer for the Internet: GENEXXO's Vision"

Content:
- Introduction to GENEXXO concept
- Link to vision page
- Explain XX-signature domains
- Link to domain portfolio
- Discuss AI opportunities
- Link to AI architecture strategy

CTA: Visit full documentation at [site URL]
```

## Deployment

### GitHub Pages

1. **Push to GitHub:**
```bash
git add .
git commit -m "Initial GENEXXO Vision site"
git push origin main
```

2. **Enable Pages:**
- Go to Settings → Pages
- Source: main branch
- Save

3. **Wait for build (2-5 minutes)**

### Custom Domain

1. **Add CNAME file:**
```bash
echo "yourdomain.com" > CNAME
```

2. **Configure DNS:**
```
Type: CNAME
Name: www
Value: [username].github.io
```

3. **Update _config.yml:**
```yaml
url: "https://yourdomain.com"
baseurl: ""
```

## Maintenance

### Regular Updates

- Add new content to collections
- Update domain portfolio
- Refresh strategy documents
- Monitor analytics
- Check broken links
- Update dependencies

### Monitoring

- **Google Search Console:** Track indexing
- **Analytics:** Monitor traffic
- **Social Media:** Track shares and engagement
- **Backlinks:** Monitor inbound links

## Performance

### Optimization Tips

1. **Compress images** before uploading
2. **Minimize CSS/JS** in production
3. **Use CDN** for static assets
4. **Enable caching** headers
5. **Monitor load times**

### Testing Performance

```bash
# Google PageSpeed Insights
https://pagespeed.web.dev/

# GTmetrix
https://gtmetrix.com/
```

## Troubleshooting

### Common Issues

**Site not building:**
- Check `_config.yml` syntax
- Verify front matter in pages
- Review GitHub Actions logs

**Links not working:**
- Check baseurl configuration
- Use `relative_url` filter
- Verify internal links

**SEO not working:**
- Verify sitemap generation
- Check robots.txt
- Validate Schema.org markup

## Advanced Features

### Adding Analytics

**Google Analytics:**
```yaml
# _config.yml
google_analytics: UA-XXXXXXXXX-X
```

**Plausible (privacy-focused):**
```html
<!-- _includes/head.html -->
<script defer data-domain="yourdomain.com" src="https://plausible.io/js/script.js"></script>
```

### Adding Search

**Jekyll Search:**
```bash
# Add to Gemfile
gem 'jekyll-algolia'

# Configure in _config.yml
algolia:
  application_id: 'your_app_id'
  index_name: 'genexxo'
```

## Support & Resources

- **Jekyll Documentation:** https://jekyllrb.com/docs/
- **GitHub Pages Guide:** https://docs.github.com/en/pages
- **Schema.org Reference:** https://schema.org/docs/gs.html
- **SEO Best Practices:** https://developers.google.com/search/docs

## License

© 2024 GENEXXO Vision Limited. All rights reserved.

## Contact

For questions or acquisition inquiries:
- Email: contact@genexxo.com
- LinkedIn: [Company Page]
- Twitter: [@genexxo]

---

**GENEXXO Vision Limited**  
*The Organizing Layer for the Internet*
