# Sveleven

Ultra-lightweight, zero-config Eleventy starter (with Tailwind & CMS included!)

<div class="flex gap-2 not-prose">
  <img src="https://img.shields.io/netlify/93494d69-cb21-4ad0-855f-3748d3741e5c">
  <img src="https://img.shields.io/github/v/release/anydigital/sveleven?include_prereleases&color=white">
  <a href="https://github.com/anydigital/sveleven"><img src="https://img.shields.io/github/stars/anydigital/sveleven"></a>
</div>

## Killer Features

1. **"Thin client" architecture**  
   <sup>thanks to [eleventy-bricks](https://github.com/anydigital/eleventy-bricks) for zero-config</sup>
2. **Dual template support**  
   <sup>`.liquid` or `.njk`, choice is yours</sup>
3. **CMS included**  
   <sup>[sveltia-cms](https://github.com/sveltia/sveltia-cms), a modern Netlify/Decap successor</sup>
4. **Tailwind CSS included**  
   <sup>with Typography plugin</sup>
5. **Multisite support**  
   <sup>thanks to symlink-based setup</sup>
6. **One-click start**  
   [![Deploy to Netlify](https://www.netlify.com/img/deploy/button.svg)](https://app.netlify.com/start/deploy?repository=https://github.com/anydigital/sveleven)

---

## First Things First

### Project Structure

All you need for _YOUR_ website is basically these 4 files:

```treeview
./src/
├── _data/site.yml              # YOUR site-wide metadata
├── _theme/__layout.**          # YOUR .liquid or .nkj template
├── _theme/styles.css           # YOUR styles (with Tailwind)
└── _public/admin/config.yml    # YOUR CMS config
```

All other files are either simple defaults, or automagically symlinked from https://github.com/anydigital/eleventy-bricks and https://github.com/anydigital/bricks :

<figure class="invert">

```treeview
./
├── eleventy.config.js          # symlinked 11ty config 🔗
├── netlify.toml                # default Netlify config
├── package.json                # default npm dependencies
├── do/package.json             # symlinked npm scripts 🔗
└── src/                        # default 11ty `input` dir
    ├── *.md                    # CMS-editable content
    ├── src.yml                 # default layout config
    ├── _theme/                 # default 11ty `includes` dir
    │   └── bricks/             # symlinked components (bricks) 🔗
    └── _public/                # default 11ty static files
        ├── media/              # CMS-managed media files
        └── admin/index.html    # symlinked Sveltia CMS 🔗
```

</figure>

Yes, `eleventy.config.js` is symlinked too, so no more JavaScript config friction!&nbsp;✨

### Local Development

```sh
npm install    # install dependencies
npm start      # start development
npm run stage  # test production version locally
               # ready to deploy! 🚀
```

CMS will be available locally at `http://localhost:8080/admin/` (or similar port).

---

## _Any_ Questions?

- Sveleven question, or rough idea? https://github.com/orgs/anydigital/discussions
  - Bug report, or specific suggestion? https://github.com/anydigital/sveleven/issues
    - Else? 11ty's Discord: https://discord.gg/qTVJvrWF4

---

## More Info

- GitHub repo: https://github.com/anydigital/sveleven
- Found it useful? Donate a ~~dollar~~ star: &nbsp;[![GitHub Repo stars](https://img.shields.io/github/stars/anydigital/sveleven?style=social)](https://github.com/anydigital/sveleven)
- Featured in:
  - https://11tybundle.dev/starters/
  - https://sveltiacms.app/en/docs/start#eleventy
- License: [MIT](https://github.com/anydigital/sveleven/blob/main/LICENSE)

### PS: Why "Sveleven"?

<pre>
SVELEVEN = <mark>SV</mark>eltia CMS
           + <mark>ELEVEN</mark>ty SSG
</pre>

"Sveleven" is simply a portmanteau of "[Sveltia CMS](https://github.com/sveltia/sveltia-cms)" and "[Eleventy SSG](https://github.com/11ty/eleventy)" — two great open-source projects that work together seamlessly.
