# Sveleven

Ultra-lightweight, zero-config Eleventy starter (with Tailwind & CMS included!)

<div class="flex gap-2 not-prose">
  <img src="https://img.shields.io/netlify/93494d69-cb21-4ad0-855f-3748d3741e5c">
  <img src="https://img.shields.io/github/v/release/anydigital/sveleven?include_prereleases&color=white">
  <a href="https://github.com/anydigital/sveleven"><img src="https://img.shields.io/github/stars/anydigital/sveleven"></a>
</div>

### Killer Features

1. **"Thin client" architecture** <br>
   <sup>thanks [eleventy-bricks](https://github.com/anydigital/eleventy-bricks) for heavy-lifting</sup>
2. **CMS included** <br>
   <sup>[sveltia-cms](https://github.com/sveltia/sveltia-cms), a modern Netlify/Decap successor</sup>
3. **Tailwind CSS included** <br>
   <sup>with Typography plugin</sup>
4. **One-click deployment to Netlify** <br>
   <sup>or any similar platform</sup>

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
├── eleventy.config.js        # default 11ty config by `eleventy-bricks` 🔗
├── netlify.toml              # default Netlify config
├── package.json              # default dependencies
├── do/package.json           # default npm scripts by `eleventy-bricks` 🔗
└── src/                      # default 11ty `input` dir
    ├── index.md            # YOUR home page (editable via CMS!)
    ├── src.yml               # default layout config
    ├── _data/site.yml      # YOUR site-wide data (title, etc.)
    ├── _template/            # default 11ty `includes` dir
    │   ├── bricks/           # default Liquid `bricks` 🔗
    │   ├── __layout.liquid # YOUR layout template
    │   └── styles.css        # default Tailwind CSS [with YOUR styles]
    └── _public/              # default 11ty static files dir
        └── admin/            # default Sveltia CMS dir
            ├── config.yml  # YOUR CMS config
            └── index.html    # default CMS html by `eleventy-bricks` 🔗
```

### Why "Sveleven"?

<pre>
SVELEVEN = <mark>SV</mark>eltia CMS
           + <mark>ELEVEN</mark>ty SSG
</pre>

"Sveleven" is simply a portmanteau of "[Sveltia CMS](https://github.com/sveltia/sveltia-cms)" and "[Eleventy SSG](https://github.com/11ty/eleventy)" — two great open-source projects that work together seamlessly.

### More Info

- Fork, try, and contribute back: https://github.com/anydigital/sveleven
- Ask questions and share ideas: https://github.com/orgs/anydigital/discussions
- Featured in: https://sveltiacms.app/en/docs/start#eleventy
- Found it useful? Donate a ~~dollar~~ star: &nbsp;[![GitHub Repo stars](https://img.shields.io/github/stars/anydigital/sveleven?style=social)](https://github.com/anydigital/sveleven)
- License: [MIT](https://github.com/anydigital/sveleven/blob/main/LICENSE)
