# Sveleven

A truly minimal, one-click Eleventy starter (with CMS included!)

[![GitHub Repo stars](https://img.shields.io/github/stars/anydigital/sveleven?style=social)](https://github.com/anydigital/sveleven)

## Killer Features

- **"Thin client" architecture** (thanks to [eleventy-bricks](https://github.com/anydigital/eleventy-bricks))
- **CMS included** ([sveltia-cms](https://github.com/sveltia/sveltia-cms), a modern Netlify/Decap successor)
- **Tailwind CSS included** (with Typography plugin)
- **One-click deployment to Netlify** (or any similar platform)

### Quick Start

[![Deploy to Netlify](https://www.netlify.com/img/deploy/button.svg)](https://app.netlify.com/start/deploy?repository=https://github.com/anydigital/sveleven)

### Local Development

```sh
npm install # Install dependencies
npm start # Start dev server
npm run stage # Build and serve production version locally
```

Ready to deploy! 🚀

### Project Structure

```
./
└── src/ -- default 11ty input dir
    └── _data/
        └── site.yml -- default 11ty config to set site-wide data
    └── _public/ -- default 11ty static files dir (for passthrough copy)
        └── admin/ -- Sveltia CMS
            ├── config.yml -- default CMS config
            └── index.html -- symlink to default CMS UI `eleventy-bricks/src/admin/index.html`
    └── _template/
        ├── bricks/ -- symlink to default Nunjucks `bricks/bricks`
        ├── __layout.njk -- default layout template
        └── styles.css -- default Tailwind CSS with Typography plugin
    ├── index.md -- this exact README file as a sample home page (fully editable via CMS!)
    └── src.yml -- default 11ty config to set layout for all pages
└── do/
    ├── package.json -- symlink to default npm scripts `eleventy-bricks/src/do/package.json`
├── package.json
├── eleventy.config.js -- symlink to default `eleventy-bricks/src/eleventy.config.js`
└── netlify.toml -- default Netlify config
```

## Why "Sveleven"?

"Sveleven" is simply a portmanteau of ["<mark>Sve</mark>ltia CMS"](https://github.com/sveltia/sveltia-cms) and ["<mark>Eleven</mark>ty"](https://github.com/11ty/eleventy) -- two great open-source projects that work together seamlessly.

### Featured In

https://sveltiacms.app/en/docs/start#eleventy

### License

MIT
