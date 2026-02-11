# Sveleven

Ultra-lightweight, modern Eleventy v4 starter (with Tailwind & CMS included!)

<div class="flex gap-2 not-prose">
  <img src="https://img.shields.io/netlify/93494d69-cb21-4ad0-855f-3748d3741e5c">
  <img src="https://img.shields.io/github/v/release/anydigital/sveleven?color=white&">
  <a href="https://github.com/anydigital/sveleven"><img src="https://img.shields.io/github/stars/anydigital/sveleven"></a>
</div>

## Killer Features

1. **Eleventy v4 by default**  
   <sup>both v4 (default) and v3 supported</sup>
2. **"Thin client" architecture**  
   <sup>thanks [eleventy-bricks](https://github.com/anydigital/eleventy-bricks) for reusability</sup>
3. **Tailwind v4 included**  
   <sup>with Typography plugin & [*Any*bricks](https://github.com/anydigital/bricks)</sup>
4. **Sveltia CMS included**  
   <sup>modern Decap/Netlify CMS successor</sup>
5. **Dual template support**  
   <sup>`.njk` or `.liquid`, choice is yours</sup>
6. **Multisite support**  
   <sup>thanks to symlink-based setup</sup>
7. **One-click start**  
   [![Deploy to Netlify](https://www.netlify.com/img/deploy/button.svg)](https://app.netlify.com/start/deploy?repository=https://github.com/anydigital/sveleven)

---

## All You Need

All you need to personalize _YOUR_ website is basically these 4 files:

```treeview
./src/
├── _data/site.yml              # YOUR site-wide metadata
├── _theme/__layout.**          # YOUR template (.njk or .liquid)
├── _theme/styles.css           # YOUR styles (with Tailwind v4)
└── _public/admin/config.yml    # YOUR CMS config
```

### Under the Hood

All other files are either simple defaults, or automagically symlinked from https://github.com/anydigital/eleventy-bricks and https://github.com/anydigital/bricks :

<figure class="invert">

```treeview
./
├── eleventy.config.js          🔗 symlinked 11ty config
├── do/package.json             🔗 symlinked npm scripts
├── package.json                # default npm dependencies
├── netlify.toml                # default Netlify config
├── .prettierrc.json            🔗 symlinked Prettier config
└── src/                        # default 11ty `input` dir
    ├── _theme/                 # default 11ty `includes` dir
    │   └── bricks/             🔗 symlinked components (bricks)
    ├── _public/                # default 11ty static files
    │   ├── admin/index.html    🔗 symlinked Sveltia CMS html
    │   ├── media/              # CMS-managed media files
    └── *.md                    # CMS-managed content
```

</figure>

Yes, `eleventy.config.js` is symlinked too, so no more JavaScript config friction!&nbsp;✨

However, you can copy any of the symlinked files over to your project, and modify them as needed.

### Local Development

```sh
npm install    # install dependencies
npm start      # start development
npm run stage  # test production version locally
               # ready to deploy! 🚀
```

CMS will be available locally at `http://localhost:8080/admin/` (or similar port).

---

## Showcase

https://any.digital/ &nbsp;
[<i class="fa-solid fa-plus text-gray-300 hover:text-black"></i>](https://github.com/anydigital/sveleven/edit/main/src/index.md){title="Suggest your website started by Sveleven"}

---

## More Info

Repository: https://github.com/anydigital/sveleven

Found it useful? Donate a ~~dollar~~ star: &nbsp;[![](https://img.shields.io/github/stars/anydigital/sveleven)](https://github.com/anydigital/sveleven)

Featured in:

- https://11tybundle.dev/starters/
- https://11tybundle.dev/blog/11ty-bundle-83/
- https://sveltiacms.app/en/docs/start#eleventy
- https://sveltiacms.app/en/docs/frameworks/eleventy
- https://any.digital/tricks/11ty/#min-starters

Support:

- https://github.com/orgs/anydigital/discussions for questions and ideas
- https://github.com/anydigital/sveleven/issues for change requests or bug reports
- https://www.11ty.dev/blog/discord/ for 11ty community support
- https://sveltiacms.app/en/support for Sveltia CMS community support

License: [MIT](https://github.com/anydigital/sveleven/blob/main/LICENSE)

### <span class="font-thin">PS:</span> Why "Sveleven"?

<pre>
SVELEVEN = <mark>SV</mark>eltia CMS
           + <mark>ELEVEN</mark>ty SSG
</pre>

"Sveleven" is simply a portmanteau of "[Sveltia CMS](https://github.com/sveltia/sveltia-cms)" and "[Eleventy SSG](https://github.com/11ty/eleventy)" — two great open-source projects that work together seamlessly.
