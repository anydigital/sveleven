# Sveleven

Ultra-lightweight, zero-config Eleventy starter (with Tailwind & CMS included!)

<div class="flex gap-2 not-prose">
  <img src="https://img.shields.io/netlify/93494d69-cb21-4ad0-855f-3748d3741e5c">
  <img src="https://img.shields.io/github/v/release/anydigital/sveleven?include_prereleases&color=white&">
  <a href="https://github.com/anydigital/sveleven"><img src="https://img.shields.io/github/stars/anydigital/sveleven"></a>
</div>

### Killer Features

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

### Project Structure

These 5 of `YOUR` files is all you need to manage:

```treeview
./
├── eleventy.config.js        # default 11ty config 🔗 from `eleventy-bricks`
├── package.json              # default dependencies
├── do/package.json           # default npm scripts 🔗 from `eleventy-bricks`
└── src/                      # default 11ty `input` dir
    ├── index.md  <— YOUR home page (editable via CMS!)    |
    ├── src.yml               # default layout config
    ├── _data/site.yml  <— YOUR site-wide data (title, etc.)    |
    ├── _theme/               # default 11ty `includes` dir
    │   ├── bricks/           # default components 🔗 from `bricks`
    │   ├── __layout.*  <— YOUR layout template    |
    │   └── styles.css  <— YOUR styles    # default Tailwind CSS included
    └── _public/              # default 11ty static files dir
        └── admin/            # default Sveltia CMS dir
            ├── config.yml  <— YOUR CMS config    |
            └── index.html    # default CMS html 🔗 from `eleventy-bricks`
```

All `default` files are either super small, or automagically symlinked from https://github.com/anydigital/eleventy-bricks.

And yes, `eleventy.config.js` is symlinked too, so no more JavaScript config friction! ✨

### Local Development

```sh
npm install    # install dependencies
npm start      # start development
npm run stage  # test production version locally
               # ready to deploy! 🚀
```

CMS will be available locally at `http://localhost:8080/admin/` (or similar port).

## More Info

- Fork, try, and contribute back: https://github.com/anydigital/sveleven
- Ask questions and share ideas: https://github.com/orgs/anydigital/discussions
- Featured in: https://sveltiacms.app/en/docs/start#eleventy
- Found it useful? Donate a ~~dollar~~ star: &nbsp;[![GitHub Repo stars](https://img.shields.io/github/stars/anydigital/sveleven?style=social)](https://github.com/anydigital/sveleven)
- License: [MIT](https://github.com/anydigital/sveleven/blob/main/LICENSE)

### PS: Why "Sveleven"?

<pre>
SVELEVEN = <mark>SV</mark>eltia CMS
           + <mark>ELEVEN</mark>ty SSG
</pre>

"Sveleven" is simply a portmanteau of "[Sveltia CMS](https://github.com/sveltia/sveltia-cms)" and "[Eleventy SSG](https://github.com/11ty/eleventy)" — two great open-source projects that work together seamlessly.
