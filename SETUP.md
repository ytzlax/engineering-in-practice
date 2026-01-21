# Setup Guide for GitHub Pages

## Quick Start (No Local Installation Needed)

You can push directly to GitHub and GitHub Pages will build your site automatically!

```bash
git add .
git commit -m "Set up GitHub Pages blog"
git push origin main
```

Then enable GitHub Pages:
1. Go to your repository on GitHub
2. Settings → Pages
3. Select "main" branch
4. Click Save
5. Wait a few minutes, then visit: `https://your-username.github.io/engineering-in-practice`

## Local Development Setup (Optional)

If you want to preview your site locally before pushing:

### Windows Installation

1. **Download RubyInstaller**
   - Visit: https://rubyinstaller.org/downloads/
   - Download "Ruby+Devkit" (recommended version: 3.2.x or 3.3.x)
   - Run the installer and follow the prompts
   - **Important**: Check "Run 'ridk install' to setup MSYS2" at the end

2. **Verify Installation**
   ```bash
   ruby --version
   gem --version
   ```

3. **Install Bundler**
   ```bash
   gem install bundler
   ```

4. **Install Dependencies**
   ```bash
   bundle install
   ```

5. **Run Local Server**
   ```bash
   bundle exec jekyll serve
   ```

6. **View Site**
   - Open browser to: http://localhost:4000

### Alternative: Use WSL (Windows Subsystem for Linux)

If you have WSL installed:
```bash
sudo apt-get update
sudo apt-get install ruby-full build-essential
gem install bundler
bundle install
bundle exec jekyll serve
```

## Troubleshooting

### "bundle: command not found"
- Ruby is not installed. Follow the Windows installation steps above.

### "Could not find gem 'github-pages'"
- Run `bundle install` to install dependencies

### Port 4000 already in use
- Use a different port: `bundle exec jekyll serve --port 4001`

## Notes

- **You don't need local Jekyll** - GitHub Pages builds automatically
- Local testing is only useful for previewing changes before pushing
- First build on GitHub Pages may take 5-10 minutes
