[sloww.org](sloww.org)

---

## ❓ What is this

A homepage for an artist.

## 🛠 Technical info

- 💚 The site is totally static and works with 0 client-site JavaScript
- And yet, the site can be easily edited through a visual interface

### Stack

- [Astro](https://astro.build/) as the static site generator (SSG)
- [Builder.io](https://builder.io/) for a low-code CMS solution, see below

### Use Case

A collaboration of a technical person with an artist with a budget of 0.
After setting up, the artist can edit the website through builder's drag-and-drop interface. She can change the content and design of the site without needing to learn the technical stuff that goes on in the background. She has full creative control and the developer can enjoy their supporting role.

### Architecture

#### An edit cycle

- Artist makes a change to the site using builder's visual editor and clicks 'publish'
- Builder triggers a re-build of the site on Netlify via a webhook
- During the rebuild Astro fetches the updated content of the site via one of Builder's APIs
- 💥 The result is a totally static site!

## 🙏 Acknowledgements

Thanks to HamatoYogi for writing his super helpful [blog article on integrating Builder with Astro](https://www.hamatoyogi.dev/blog/astro-log/connecting-builderio-to-astro)!

Thanks to the Astro and Builder communities on Discord and the forums for all the support!
