# Alto (Pro Profile Fork)

(This is a fork of Ghost's alto theme, for use as a simple professional profile. It is aimed towards people who code for a living.)

Fork features/focus:

* Remove cruft that wouldn't make sense on a professional profile page (e.g. reading time on blog posts).
* Simple featured posts. Use them to welcome visitors to your site or post important messages, that's it.


--------------------------------
(Standard alto readme below here)

* Pages show "updated at" dates so if you forget to update your "About me site" for a few years, there's no confusion.

A clean, minimalist theme featuring a light and dark mode. Launch your online publications with flair. Completely free and fully responsive, released under the MIT license.

**Demo: https://alto.ghost.io**

&nbsp;

# Instructions

1. [Download this theme](https://github.com/TryGhost/Alto/archive/main.zip)
2. Log into Ghost, and go to the `Design` settings area to upload the zip file

# White Logo

If your logo image isn't recognizable in dark mode, you can set a white version of the logo in `Code injection > Site Header` field.

```html
<script>
    var gh_white_logo = 'https://example.com/content/images/white-logo.png';
</script>
```

# Development

Styles are compiled using Gulp/PostCSS to polyfill future CSS spec. You'll need [Node](https://nodejs.org/), [Yarn](https://yarnpkg.com/) and [Gulp](https://gulpjs.com) installed globally. After that, from the theme's root directory:

```bash
# Install
yarn

# Run build & watch for changes
$ yarn dev
```

Now you can edit `/assets/css/` files, which will be compiled to `/assets/built/` automatically.

The `zip` Gulp task packages the theme files into `dist/<theme-name>.zip`, which you can then upload to your site.

```bash
yarn zip
```

# PostCSS Features Used

-   Autoprefixer - Don't worry about writing browser prefixes of any kind, it's all done automatically with support for the latest 2 major versions of every browser.

# Copyright & License

Copyright (c) 2013-2022 Ghost Foundation - Released under the [MIT license](LICENSE).
