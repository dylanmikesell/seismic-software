# Seismic Processing Tools - Site Maintenance Guide

This repository hosts a GitHub Pages site that serves as a comprehensive resource for open-source seismic data analysis and modeling tools. This guide will help you maintain and update the site.

## Site Structure

```
seismic-software/
├── _config.yml           # Jekyll configuration
├── _layouts/             # HTML templates
│   ├── default.html      # Main site layout
│   └── page.html         # Page layout
├── _sass/                # CSS stylesheets
│   └── academic-blue.scss # Main theme
├── assets/css/           # Compiled CSS
│   └── main.scss         # CSS entry point
├── index.md              # Homepage
├── first-break-analysis.md # Example method page
├── Gemfile              # Ruby dependencies
└── README.md            # This file
```

## Quick Start

### Local Development

1. **Install Ruby and Jekyll** (if not already installed):
   ```bash
   # On Ubuntu/Debian
   sudo apt-get install ruby-full build-essential zlib1g-dev
   
   # On macOS with Homebrew
   brew install ruby
   ```

2. **Install dependencies**:
   ```bash
   cd /path/to/seismic-software
   bundle install
   ```

3. **Serve the site locally**:
   ```bash
   bundle exec jekyll serve
   ```
   
   The site will be available at `http://localhost:4000/seismic-software/`

### Deploy to GitHub Pages

1. **Push changes to GitHub**:
   ```bash
   git add .
   git commit -m "Update site content"
   git push origin main
   ```

2. **Enable GitHub Pages** (one-time setup):
   - Go to your repository on GitHub
   - Navigate to Settings → Pages
   - Under "Source", select "Deploy from a branch"
   - Select "main" branch and "/ (root)" folder
   - Click "Save"

3. **Access your site**:
   - Your site will be available at: `https://dylanmikesell.github.io/seismic-software/`
   - It may take a few minutes for changes to appear

## Adding New Tools

### Method 1: Edit Existing Method Pages

To add a tool to an existing method page (e.g., `first-break-analysis.md`):

1. **Open the method page** in your editor
2. **Copy the tool template** (found at the bottom of each method page)
3. **Fill in the tool information**:
   - Tool name and description
   - Maintenance status (`maintained`, `unmaintained`, or `unknown`)
   - Programming language and license
   - Key features
   - GitHub URL and documentation links
4. **Save and commit** your changes

### Method 2: Create New Method Pages

To create a new method category:

1. **Create a new markdown file**: `new-method-name.md`
2. **Add front matter**:
   ```yaml
   ---
   layout: page
   title: "Your Method Name"
   permalink: /your-method-name/
   ---
   ```
3. **Follow the structure** of `first-break-analysis.md`
4. **Update navigation** in `_layouts/default.html` and `index.md`

## Site Customization

### Colors and Styling

The site uses a professional blue color scheme defined in `_sass/academic-blue.scss`:

- **Primary Blue**: #1e3a8a (headers, navigation)
- **Secondary Blue**: #3b82f6 (buttons, accents)
- **Light Blue**: #dbeafe (backgrounds, highlights)

To modify colors, edit the variables at the top of `_sass/academic-blue.scss`.

### Adding New Sections

To add new content sections to the homepage:

1. **Edit** `index.md`
2. **Add your content** using Markdown
3. **Use CSS classes** from the theme (e.g., `method-nav`, `tool-card`)

### Typography

The site uses:
- **Headers**: Source Serif Pro (academic feel)
- **Body text**: Source Sans Pro (readability)
- **Code**: Monaco/Menlo (monospace)

## Content Guidelines

### Tool Evaluation Criteria

When adding tools, consider:

- **Code Quality**: Good documentation, testing, clean structure
- **Maintenance**: Recent commits, active issue responses
- **Usability**: Easy installation, examples, tutorials
- **Performance**: Computational efficiency
- **Community**: User base, academic citations

### Maintenance Status Guidelines

- **Actively Maintained**: Regular commits (within 6 months), active issues/PRs
- **Unmaintained**: No activity for 1+ years, unresponsive maintainers
- **Unknown**: Unclear maintenance status, requires investigation

### Writing Style

- Use **clear, concise descriptions**
- Focus on **practical benefits** for researchers
- Include **technical requirements** and dependencies
- Provide **installation guidance** where possible
- Use **academic tone** appropriate for scientific audience

## Troubleshooting

### Common Issues

1. **Jekyll build fails**:
   - Check for YAML front matter syntax errors
   - Ensure all required fields are present
   - Validate markdown syntax

2. **CSS not updating**:
   - Clear browser cache
   - Check that `main.scss` imports are correct
   - Restart Jekyll server

3. **GitHub Pages not updating**:
   - Check GitHub Actions tab for build errors
   - Ensure all commits are pushed to main branch
   - Wait 5-10 minutes for propagation

### Getting Help

- **Jekyll Documentation**: https://jekyllrb.com/docs/
- **GitHub Pages**: https://docs.github.com/en/pages
- **Markdown Guide**: https://www.markdownguide.org/

## File Templates

### New Method Page Template

```markdown
---
layout: page
title: "Method Name"
permalink: /method-name/
---

# Method Name Tools

Brief description of the method and its applications in seismic processing.

## Available Tools

---

<div class="tool-card">
  <div class="tool-header">
    <h3 class="tool-title">Tool Name</h3>
    <span class="tool-status maintained">Actively Maintained</span>
  </div>
  
  <div class="tool-meta">
    <div class="tool-meta-item">
      <strong>Language:</strong> Python
    </div>
    <div class="tool-meta-item">
      <strong>License:</strong> MIT
    </div>
    <div class="tool-meta-item">
      <strong>Institution:</strong> University/Company
    </div>
    <div class="tool-meta-item">
      <strong>Last Updated:</strong> 2024
    </div>
  </div>
  
  <div class="tool-description">
    <p>Tool description...</p>
  </div>
  
  <div class="tool-features">
    <h4>Key Features:</h4>
    <ul>
      <li>Feature 1</li>
      <li>Feature 2</li>
    </ul>
  </div>
  
  <div class="tool-links">
    <a href="GITHUB_URL" class="btn btn-primary" target="_blank">View on GitHub</a>
    <a href="DOCS_URL" class="btn btn-secondary" target="_blank">Documentation</a>
  </div>
</div>

---

## Contributing New Tools

Instructions for adding tools to this method page...
```

## Maintenance Schedule

### Regular Tasks

- **Monthly**: Check for new tools and updates
- **Quarterly**: Verify maintenance status of listed tools
- **Annually**: Review and update site structure and design

### Monitoring

- **GitHub Stars/Activity**: Track popularity and development
- **User Feedback**: Monitor issues and suggestions
- **Academic Publications**: Watch for new tool releases in literature

---

## Contact

For questions about site maintenance or content, please:

1. **Create an issue** in the GitHub repository
2. **Submit a pull request** with improvements
3. **Contact the maintainer** directly if needed

---

*This documentation was last updated: October 2025*