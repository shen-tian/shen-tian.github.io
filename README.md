# shen-tian.github.io

Personal github page. 

## Local Development Setup

### Ruby Environment Setup (rbenv)

This project uses Ruby 2.7.8. To set up your local development environment:

1. **Install rbenv** (if not already installed):
   ```bash
   # macOS with Homebrew
   brew install rbenv
   
   # Or follow installation instructions at https://github.com/rbenv/rbenv#installation
   ```

2. **Install the required Ruby version**:
   ```bash
   rbenv install 2.7.8
   ```

3. **Set the local Ruby version** (this should already be configured via `.ruby-version`):
   ```bash
   rbenv local 2.7.8
   ```

4. **Install dependencies**:
   ```bash
   bundle install
   ```

### Running the Site

To run the site locally:

```bash
bundle exec jekyll serve
```

Then go to `localhost:4000`.

Currently using the default minima theme via a Gemfile, keeping things simple.
