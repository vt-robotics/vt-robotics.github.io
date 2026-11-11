# vt-robotics.github.io
Website for robotics at Virginia Tech: https://robotics.me.vt.edu

The site is built with [Jekyll](https://jekyllrb.com/). GitHub Pages builds it on every push to `main`.

## Editing

| To change | Edit |
| --- | --- |
| Faculty on the People page | `_data/people.yml` (portraits go in `assets/images/people/`) |
| Home page text and photo | `index.html` (photo in `assets/images/`) |
| Symposium page | `vrs.html` |
| Header, navigation, footer | `_layouts/default.html` |
| Fonts, colors, spacing | `assets/css/main.css` |

## Previewing on your computer

One-time setup (Ubuntu). Install Ruby and Bundler, then install the site's gems into `vendor/`:

```bash
sudo apt install ruby-full build-essential
gem install --user-install bundler
export PATH="$HOME/.local/share/gem/ruby/3.2.0/bin:$PATH"
bundle config set --local path vendor/bundle
bundle install
```

After that, from this folder:

```bash
~/.local/share/gem/ruby/3.2.0/bin/bundle exec jekyll serve
```

and open http://localhost:4000. Pages rebuild when you save a file. Restart the command after editing `_config.yml`.

## Credits

The font is [TeX Gyre Pagella](https://www.gust.org.pl/projects/e-foundry/tex-gyre/pagella), released under the GUST Font License.
