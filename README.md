# Yiqiao Jin — personal website

Source for my academic website, **<https://jdmunkjoey.github.io/personal-website/>**.

I am a Ph.D. student in Statistics at Washington University in St. Louis. The site covers my research, publications, talks, teaching, and CV.

The site is built with [Jekyll](https://jekyllrb.com/) and the [al-folio](https://github.com/alshedivat/al-folio) v1.x starter. Layouts, styles, and features come from versioned `al_*` gems (for example `al_folio_core`), so this repository only holds configuration and content.

## Where things live

| What                                 | File(s)                                                                                                |
| ------------------------------------ | ------------------------------------------------------------------------------------------------------ |
| Name, site URL, SEO, feature toggles | [`_config.yml`](_config.yml)                                                                           |
| Home page (bio, address, photo)      | [`_pages/about.md`](_pages/about.md), photo in `assets/img/`                                           |
| News on the home page                | [`_news/`](_news/), one Markdown file per item                                                         |
| Publications                         | [`_bibliography/papers.bib`](_bibliography/papers.bib) (`selected = {true}` shows it on the home page) |
| Talks                                | [`_pages/talks.md`](_pages/talks.md)                                                                   |
| Teaching                             | [`_pages/teaching.md`](_pages/teaching.md)                                                             |
| CV page                              | [`_data/cv.yml`](_data/cv.yml), rendered by [`_pages/cv.md`](_pages/cv.md)                             |
| CV PDF (download link)               | [`assets/pdf/Yiqiao_Jin_CV.pdf`](assets/pdf/Yiqiao_Jin_CV.pdf)                                         |
| Social / contact icons               | [`_data/socials.yml`](_data/socials.yml)                                                               |

The profile photo is `assets/img/prof_pic.jpg`; replace that file to change it. The CV PDF is maintained by hand, so update `assets/pdf/Yiqiao_Jin_CV.pdf` whenever `_data/cv.yml` changes.

## Preview locally

```bash
bundle install
bundle exec jekyll serve
```

Then open <http://localhost:4000/personal-website/>. Responsive images need ImageMagick's `convert` on your `PATH` (`imagemagick.enabled` in `_config.yml`). [`docs/INSTALL.md`](docs/INSTALL.md) covers the rest of the setup.

## Deploy

Every push to `main` that changes site content (pages, data, assets, or config) runs [`.github/workflows/deploy.yml`](.github/workflows/deploy.yml), which builds the site and publishes it to the `gh-pages` branch. You can also run it by hand from the **Actions** tab. One-time GitHub setup:

1. **Settings → Actions → General → Workflow permissions**: select **Read and write permissions**.
2. **Settings → Pages → Build and deployment**: set **Source** to **Deploy from a branch**, then choose `gh-pages` and `/ (root)`.

To serve the site from `https://jdmunkjoey.github.io/` instead, rename the repository to `jdmunkjoey.github.io`, set `baseurl:` to empty in `_config.yml`, and update the site URL in `website:` in `_data/cv.yml` and at the top of this README.

## Customization reference

[`docs/CUSTOMIZE.md`](docs/CUSTOMIZE.md) covers the options, such as adding a blog, Google Scholar citation counts, or analytics. [`docs/README.md`](docs/README.md) indexes all guides.

## License

The al-folio starter is released under the [MIT License](LICENSE).
