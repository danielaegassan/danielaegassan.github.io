# danielaegassan.github.io

Personal website, built by GitHub Pages with Jekyll. There is nothing to install: edit a file, commit, and GitHub rebuilds the site within a minute or two.

## Where things are

| To change…                    | Edit                          |
|-------------------------------|-------------------------------|
| Home page text and videos     | `index.md`                    |
| Publications                  | `research.md`                 |
| Organized events              | `conferences-and-seminars.md` |
| Talks                         | `talks.md`                    |
| Teaching                      | `teaching.md`                 |
| Contact links and photo       | `contact.md`                  |
| Menu items and their order    | `_data/navigation.yml`        |
| Colors, fonts, spacing        | `assets/css/style.css`        |
| Page frame (header, menu)     | `_layouts/default.html`       |

Images live in `assets/images/`. Reference them as `/assets/images/name.jpg`.

## Adding a page

Create `something.md` starting with

```
---
layout: default
title: Something
permalink: /something/
---
```

and add it to `_data/navigation.yml` if it should appear in the menu.

## Previewing on your computer

Uses Homebrew's Ruby by full path, so your default `ruby` and `PATH` stay unchanged.
(On an Intel Mac, replace `/opt/homebrew` with `/usr/local`.)

Once, from this folder:

```sh
brew install ruby
/opt/homebrew/opt/ruby/bin/bundle install
```

Each time, from this folder:

```sh
/opt/homebrew/opt/ruby/bin/bundle exec jekyll serve --livereload
```

Then open http://localhost:4000. Stop with Ctrl-C.

## Editing in the browser

On github.com, open a file, press the pencil icon, edit, and commit. The Actions tab shows the build; the site updates when it turns green.
