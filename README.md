Hugo theme used in broch.tech.

To use, add the following to `config.toml`.

```toml
[module]
  [[module.imports]]
  path = 'github.com/broch/broch-theme'
```

Then run

```
hugo mod npm pack
npm install
```

to create the `package.json` file for your project and setup tailwind/postcss.

## Customization

The title on the `posts` page can be set using the `blogTitle` site parameter:

```toml
[params]
  description = "My site on stuff I'm interested in and other stuff too..."
  blogTitle = "I have so much to say about everything"
```

You'll probably want to override:

- layouts/partials/analytics.html
- layouts/partials/posts-blurb.html (text that goes in /posts)
- layouts/partials/logo.html (the logo used in the navbar template)
- static/images/logo.svg (used for the site icon)

The default logos are borrowed from Rust.
