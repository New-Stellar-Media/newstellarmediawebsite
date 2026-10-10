# New Stellar Media — Static Website

A lightweight, modern, and minimal static website for **New Stellar Media**, built with [Jekyll](https://jekyllrb.com/).

## Project Structure

```text
├── _config.yml         # Jekyll configuration (title, URL, metadata)
├── Gemfile             # Ruby gem dependencies (jekyll, webrick)
├── _includes/
│   ├── header.html     # Reusable site navigation header
│   └── footer.html     # Reusable footer
├── _layouts/
│   ├── default.html    # Master HTML template
│   ├── page.html       # Layout for static pages
│   └── post.html       # Layout for blog posts / dispatches
├── _posts/
│   └── 2026-10-09-introducing-new-stellar-media.md # Inaugural dispatch
├── assets/
│   └── css/
│       └── style.css   # Modern, responsive CSS styling
├── index.html          # Homepage with hero, pillars & dispatches
├── about.md            # About New Stellar Media page
├── contact.md          # Contact & editorial inquiry page
└── README.md
```

## Running Locally

### 1. Prerequisites (macOS)
Jekyll requires Ruby (Ruby 3.1+ recommended). If using Homebrew:

```bash
brew install ruby
```

Add brew's Ruby to your PATH (if not already configured):
```bash
echo 'export PATH="/opt/homebrew/opt/ruby/bin:$PATH"' >> ~/.zshrc
source ~/.zshrc
```

### 2. Install Dependencies

Install Bundler and the project gems:

```bash
bundle install
```

### 3. Start the Local Server

```bash
bundle exec jekyll serve
```

Open [http://localhost:4000](http://localhost:4000) in your browser. Live reloading is enabled by default!

## How to Customize

- **Site settings**: Edit `_config.yml` to change the site title, email, or URL.
- **Add pages**: Create any `.md` or `.html` file with `layout: page` front matter in the root directory.
- **Add blog posts**: Add `.md` files in `_posts/` with the filename format `YYYY-MM-DD-title.md`.
- **Change styling**: Modify `assets/css/style.css` to update color tokens, typography, or spacing.
