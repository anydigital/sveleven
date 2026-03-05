# Sveleven

Modern, lightweight Eleventy v4 starter with Tailwind or Pico.css, CMS and multisiting 🥷

![](https://img.shields.io/github/v/release/anydigital/sveleven?color=black&label=)
![](https://img.shields.io/netlify/93494d69-cb21-4ad0-855f-3748d3741e5c?logo=netlify&labelColor=black&label=)
[![](https://img.shields.io/github/stars/anydigital/sveleven?label=GitHub)](https://github.com/anydigital/sveleven)

## Killer features

1. **Eleventy v4 by default**  
   <sup>both v4 (default) & v3 supported</sup>
2. **"Thin client" architecture**  
   <sup>thanks [eleventy-bricks](https://github.com/anydigital/eleventy-bricks) for reusability</sup>
3. **Tailwind v4 included**  
   <sup>with Typography plugin & <i class="fa-solid fa-cube fa-rotate-90"></i> [bricks](https://github.com/anydigital/bricks) theme</sup>
4. **Sveltia CMS included**  
   <sup>modern Decap/Netlify CMS successor</sup>
5. **Multisite support**  
   <sup>thanks to symlink-based setup</sup>
6. **One-click start**  
   [![Deploy to Netlify](https://www.netlify.com/img/deploy/button.svg)](https://app.netlify.com/start/deploy?repository=https://github.com/anydigital/sveleven)

---

## How it works?

**Sveleven** is an advanced version of 🥷 [*Blade*switch](https://bladeswitch.com/) starter:

- _BUT_ focusing exclusively on Eleventy v4 and adding Tailwind v4 support.
- It uses same [eleventy-bricks](https://github.com/anydigital/eleventy-bricks) plugin to symlink `eleventy.config.js` by default (so you don't have to maintain it anymore!)
- It also uses Nunjucks version of the same _universal_ <i class="fa-solid fa-cube fa-rotate-90"></i> [bricks](https://github.com/anydigital/bricks) theme:
  - _universal_ means you can switch `.njk` to `.liquid` any time
  - _universal_ also means you can switch from `tailwind` to `pico.css` or even bare-metal `bricks.css`

---

## Local development

As simple as:

```sh
npm install    # dependencies
npm start      # development
npm run stage  # serve production version locally
               # ready to deploy! 🚀
```

CMS will be available locally at `http://localhost:8080/admin/` (or similar port).

---

## Showcase

https://any.digital/ &nbsp;
[<i class="fa-solid fa-plus text-gray-300 hover:text-black"></i>](https://github.com/anydigital/sveleven/edit/main/src/index.md){title="Suggest your website started by Sveleven"}

---

## More info

<big>Repository: https://github.com/anydigital/sveleven</big>

Found it useful? Give a [![](https://img.shields.io/github/stars/anydigital/sveleven?label=Star)](https://github.com/anydigital/sveleven)

Featured in:

- https://11tybundle.dev/starters/
- https://11tybundle.dev/blog/11ty-bundle-83/
- https://www.11ty.dev/docs/starter/
- https://sveltiacms.app/en/docs/start#starter-templates
- https://sveltiacms.app/en/docs/frameworks/eleventy
- https://any.digital/tricks/11ty/#min-starters
- https://bladeswitch.com starter
- https://github.com/anydigital/awesome-11ty-build-awesome

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
