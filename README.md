# welcome-to-cdocs
This is the docs repository strictly for Casey Brown. You can leave a comment if you'd like, but no contributors are allowed :)

## About

This repository holds the source for Casey Brown's technical writing portfolio, published at **https://caseybrown.world**.

The site is built with [Jekyll](https://jekyllrb.com/) and hosted on [GitHub Pages](https://pages.github.com/). It uses the [portfolYOU](https://github.com/yousinix/portfolYOU) remote theme, with a custom navigation bar and styles layered on top.

## Repository structure

```
.
├── _config.yml               # Site settings: title, URL, baseurl, theme, plugins
├── _data/
│   └── navigation.yml        # Top navigation drop-down menus and their links
├── _includes/
│   └── navbar.html           # Replaces the theme's navbar; builds menus from navigation.yml
├── assets/
│   └── css/style.scss        # Custom styles applied on top of the theme
├── images/                   # Images used on the site (headshot, diagrams)
├── js/                       # Custom JavaScript
├── index.md                  # Home page
├── pages/
│   └── about.md              # About me page (/about/)
├── projects/                 # Portfolio projects (documentation plan, IA project)
├── writing-samples/          # Writing samples (docs-as-code articles)
├── docs/                     # Placeholder for future docs projects
├── styles/                   # Vale style packages: Google, proselint, alex, Readability
├── .vale.ini                 # Vale configuration (which styles apply to which files)
├── .github/workflows/
│   └── vale.yml              # Runs Vale on every push and pull request
├── CODEOWNERS                # Requires review from @caseyabrown on all changes
├── Gemfile / Gemfile.lock    # Ruby dependencies (pinned to the GitHub Pages versions)
└── README.md
```

The following folders are generated locally and ignored by Git, so don't edit or commit them:

| Folder | What it is |
| --- | --- |
| `_site/` | The built website that Jekyll outputs. It's rebuilt on every build. |
| `.jekyll-cache/` | Jekyll's build cache. |
| `vendor/`, `.bundle/` | Locally installed Ruby gems and Bundler settings. |

## Run the site locally

Prerequisites: [Ruby](https://www.ruby-lang.org/) and [Bundler](https://bundler.io/).

1. Install the dependencies:

   ```sh
   bundle install
   ```

2. Start the local server:

   ```sh
   bundle exec jekyll serve
   ```

3. Open http://localhost:4000/ in your browser. The site rebuilds automatically when you save a file, except for changes to `_config.yml`, which require restarting the server.

## Add a page

1. Create a Markdown file in the right folder (for example, `writing-samples/my-new-sample.md`) and start it with front matter:

   ```yaml
   ---
   layout: page
   title: My new sample
   permalink: /writing-samples/my-new-sample/
   ---
   ```

2. To show the page in the navigation bar, add it under the right menu in `_data/navigation.yml`:

   ```yaml
   - title: Writing samples
     children:
       - title: My new sample
         url: /writing-samples/my-new-sample/
   ```

3. Link to images and other pages with the `relative_url` filter so links keep working if a base path is ever configured:

   ```md
   ![Description of the image]({{ '/images/my-image.png' | relative_url }})
   [Another page]({{ '/writing-samples/another-page/' | relative_url }})
   ```

   A plain relative path such as `images/my-image.png` resolves against the page's own URL and breaks.

## Style checks

[Vale](https://vale.sh/) checks every Markdown file against the Google developer documentation style guide, `proselint`, `alex` (inclusive language), and readability rules. The GitHub Actions workflow runs it on every push and pull request.

To run it locally, [install Vale](https://vale.sh/docs/install) and run:

```sh
vale .
```

## Publishing

GitHub Pages builds and publishes the site from the `main` branch. Changes go live a few minutes after they're merged.

© 2026 Casey Brown. All rights reserved.
