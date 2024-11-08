# Godot Game Settings Documentation

The documentation for the [Godot Game Settings](https://github.com/PunchablePlushie/godot-game-settings), a plugin for Godot game engine.

Made with [mdBook](https://github.com/rust-lang/mdBook), along with the following third-party plugins:

- [mdbook-admonish](https://github.com/tommilligan/mdbook-admonish)
- [mdbook-pagetoc](https://github.com/slowsage/mdbook-pagetoc)

## Content Guide

- **docs**: The output of mdbook which is the final rendered docs.
- **src**: The actual content of the docs. Mdbook uses the markdown files here to build the docs.
  - **SUMMARY.md**: The navigation panel to the left.
- **theme**
  - **favicon.png/svg**: The tab icon of the docs.
  - **index.hbs**: The [Handlebars](https://handlebarsjs.com/) file mdbook uses to layout the docs.
  - **mdbook-admonish.css**: Used by the mdbook-admonish plugin.
  - **mdbook-pagetoc.css/js**: Used by the mdbook-pagetoc plugin.
  - **.prettierignore**: Prevents Prettier from messing with certain markdown files if using VSCode.
  - **book.toml**: Mdbook configuration.
