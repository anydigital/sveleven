# Sveleven

A truly minimal, one-click Eleventy starter (with CMS included!)

### Killer Features

- **"Thin client" architecture** (thanks [eleventy-bricks](https://github.com/anydigital/eleventy-bricks) for heavy-lifting)
- **CMS included** ([sveltia-cms](https://github.com/sveltia/sveltia-cms), a modern Netlify/Decap successor)
- **Tailwind CSS included** (with Typography plugin)
- **One-click deployment to Netlify** (or any similar platform)

### Quick Start

[![Deploy to Netlify](https://www.netlify.com/img/deploy/button.svg)](https://app.netlify.com/start/deploy?repository=https://github.com/anydigital/sveleven)

## Local Development

```sh
npm install    # install dependencies
npm start      # start development
npm run stage  # test production version locally
               # ready to deploy! 🚀
```

CMS will be available locally at `http://localhost:8080/admin/` (or similar port)

### Project Structure

```
./
├── eleventy.config.js        # default 11ty config by `eleventy-bricks` (linked)
├── netlify.toml              # default Netlify config
├── package.json              # default dependencies
├── do/package.json           # default npm scripts by `eleventy-bricks` (linked)
└── src/                      # default 11ty `input` dir
    ├── index.md            # YOUR home page (editable via CMS!)
    ├── src.yml               # default layout config
    ├── _data/site.yml      # YOUR site-wide data (title, etc.)
    ├── _template/            # default 11ty `includes` dir
    │   ├── bricks/           # default Nunjucks `bricks` (linked)
    │   ├── __layout.njk    # YOUR layout template
    │   └── styles.css        # default Tailwind CSS [with YOUR styles]
    └── _public/              # default 11ty static files dir
        └── admin/            # default Sveltia CMS dir
            ├── config.yml  # YOUR CMS config
            └── index.html    # default CMS UI (linked)
```

### Why "Sveleven"?

"Sveleven" is simply a portmanteau of ["<mark>Sve</mark>ltia CMS"](https://github.com/sveltia/sveltia-cms) and ["<mark>Eleven</mark>ty"](https://github.com/11ty/eleventy) -- two great open-source projects that work together seamlessly.

### More Info

- Fork, try, and contribute back: https://github.com/anydigital/sveleven
- Ask questions and share ideas: https://github.com/orgs/anydigital/discussions
- Featured in: https://sveltiacms.app/en/docs/start#eleventy
- Found it useful? Donate a ~~dollar~~ star: &nbsp;[![GitHub Repo stars](https://img.shields.io/github/stars/anydigital/sveleven?style=social)](https://github.com/anydigital/sveleven)
- License: [MIT](https://github.com/anydigital/sveleven/blob/main/LICENSE)
