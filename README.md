# econtanaka.github.io

Source for [econtanaka.github.io](https://econtanaka.github.io/) — Satoshi Tanaka's
academic homepage. Built with the [Minimal Light](https://github.com/yaoyao-liu/minimal-light)
Jekyll theme and served via GitHub Pages.

## Editing content

| What you want to change                                | File                               |
| ------------------------------------------------------ | ---------------------------------- |
| Name, title, affiliation, email, social/CV links       | `_config.yml`                      |
| About / Research Interests / Research Grants           | `index.md`                         |
| Publications, working papers, work-in-progress entries | `_data/publications.yml`           |
| Profile photo                                          | `assets/img/avatar.png` (replace)  |
| CV PDF                                                 | `assets/files/cv.pdf` (replace)    |
| Favicon (light/dark)                                   | `assets/img/favicon{,-dark}.png`   |

To add a new publication, add an entry under `main:` in `_data/publications.yml`:

```yaml
  - title: Your Paper Title
    authors: with Coauthor One and Coauthor Two
    conference: "<em>Journal Name</em>, Vol. X, No. Y, pp. NN-MM, Month YYYY."
    pdf: https://link-to-pdf  # optional
```

Quote any `conference:` value that contains a colon (`:`).

## Local preview (optional)

GitHub Pages builds the site automatically on every push to `main`. To preview
locally, you need Ruby plus `ruby-dev`/`build-essential` (Linux):

```bash
sudo apt install ruby-dev build-essential   # one-time, Debian/Ubuntu
bundle install
bundle exec jekyll serve
```

The site will be at <http://localhost:4000>.

## License

Content (text, publications data) © Satoshi Tanaka.
Theme: [Minimal Light](https://github.com/yaoyao-liu/minimal-light) by Yaoyao Liu (MIT).
