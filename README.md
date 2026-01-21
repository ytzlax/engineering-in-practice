# Engineering in Practice

A GitHub Pages blog sharing real-world development experiences and technical insights.

🌐 **Live Site**: [https://your-username.github.io/engineering-in-practice](https://your-username.github.io/engineering-in-practice)

## About

This blog documents hands-on experiences from real projects, covering topics like:
- IoT and Embedded Systems
- LoRaWAN Development
- Software Engineering
- Hardware Design
- System Architecture

## Local Development

To run the site locally:

1. **Install Ruby and Bundler** (if you haven't already)
   - Windows: Download from [RubyInstaller](https://rubyinstaller.org/)
   - Mac: `brew install ruby`
   - Linux: `sudo apt-get install ruby-full`

2. **Install dependencies**
   ```bash
   bundle install
   ```

3. **Run the site**
   ```bash
   bundle exec jekyll serve
   ```

4. **View in browser**
   Open `http://localhost:4000`

## Adding New Posts

Create a new file in the `_posts` directory with the format:
```
YYYY-MM-DD-title-of-post.md
```

Use this front matter template:
```yaml
---
layout: post
title: "Your Post Title"
date: YYYY-MM-DD
categories: [Category1, Category2]
tags: [tag1, tag2, tag3]
reading_time: 5
excerpt: "A brief description of your post"
---

Your content here...
```

## Enabling GitHub Pages

1. Push this repository to GitHub
2. Go to your repository Settings
3. Navigate to "Pages" in the left sidebar
4. Under "Source", select the `main` branch
5. Click "Save"
6. Your site will be available at `https://your-username.github.io/engineering-in-practice`

## Customization

- **Site info**: Edit `_config.yml`
- **Styling**: Modify `assets/css/style.scss`
- **Layouts**: Update files in `_layouts/`
- **About page**: Edit `about.md`

## Structure

```
.
├── _config.yml          # Site configuration
├── _layouts/            # Page templates
│   ├── default.html
│   ├── home.html
│   └── post.html
├── _posts/              # Blog posts
│   └── 2026-01-21-lorawan-development-experience.md
├── assets/
│   └── css/
│       └── style.scss   # Custom styles
├── index.md             # Home page
├── about.md             # About page
└── Gemfile              # Ruby dependencies
```

## Contributing

This is a personal blog, but if you spot any issues or have suggestions, feel free to open an issue!

## License

Content is mine, but feel free to use the site structure and design for your own blog.