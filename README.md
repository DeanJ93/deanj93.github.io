# Dev With Dean - Personal Blog & Portfolio

A Jekyll-powered personal website and blog showcasing programming projects and sharing development insights.

## 🌐 Live Site

Visit the live site at [devwithdean.com](https://devwithdean.com)

## 📋 Features

- **Blog**: Write and publish blog posts in Markdown
- **Projects Portfolio**: Showcase of development projects
- **Responsive Design**: Mobile-friendly layout
- **SEO Optimized**: Meta tags, Open Graph, and sitemap
- **RSS Feed**: Subscribe to blog updates
- **Tag & Category System**: Organized content navigation
- **Social Media Integration**: Links to Twitter, Instagram, Reddit, and GitHub

## 🛠️ Built With

- **Jekyll 4.3** - Static site generator
- **Sass/SCSS** - Modular stylesheets
- **GitHub Pages** - Hosting platform
- **Markdown** - Content writing format

## 📁 Project Structure

```
deanj93.github.io/
├── _config.yml           # Jekyll configuration
├── _data/                # Data files (projects, etc.)
├── _includes/            # Reusable components
│   ├── header.html
│   ├── footer.html
│   └── navigation.html
├── _layouts/             # Page templates
│   ├── default.html
│   ├── home.html
│   ├── page.html
│   └── post.html
├── _posts/               # Blog posts
│   └── YYYY-MM-DD-title.md
├── _sass/                # Sass partials
│   ├── _variables.scss
│   ├── _base.scss
│   ├── _header.scss
│   ├── _footer.scss
│   ├── _navigation.scss
│   ├── _pages.scss
│   ├── _blog.scss
│   └── _post.scss
├── assets/
│   ├── css/
│   │   └── main.scss
│   └── images/
├── blog/                 # Blog listing page
│   └── index.html
├── about.md              # About page
├── projects.html         # Projects page
├── categories.html       # Categories archive
├── tags.html             # Tags archive
├── 404.html              # Custom 404 page
├── robots.txt            # SEO robots file
├── CNAME                 # Custom domain
└── index.html            # Homepage
```

## 🚀 Getting Started

### Prerequisites

- Ruby 2.7 or higher
- Bundler gem
- Git

### Local Development

1. **Clone the repository**
   ```bash
   git clone https://github.com/DeanJ93/deanj93.github.io.git
   cd deanj93.github.io
   ```

2. **Install dependencies**
   ```bash
   bundle install
   ```

3. **Run the development server**
   ```bash
   bundle exec jekyll serve
   ```

4. **View the site**
   Open your browser and navigate to `http://localhost:4000`

The site will automatically rebuild when you make changes to files. Refresh your browser to see updates.

## ✍️ Creating Blog Posts

### Step 1: Create a New Post File

Create a new Markdown file in the `_posts` directory with the naming format:
```
YYYY-MM-DD-title-of-post.md
```

**Example**: `2026-05-21-my-first-post.md`

### Step 2: Add Front Matter

Start your post with YAML front matter:

```yaml
---
layout: post
title: "Your Post Title"
date: 2026-05-21 10:00:00 -0500
categories: [category1, category2]
tags: [tag1, tag2, tag3]
excerpt: "A brief description of your post that appears in listings."
---
```

### Step 3: Write Your Content

Below the front matter, write your content in Markdown:

```markdown
## Heading

This is a paragraph with **bold** and *italic* text.

### Subheading

- List item 1
- List item 2

```python
# Code block
def hello_world():
    print("Hello, World!")
```

[Link text](https://example.com)
```

### Step 4: Preview and Publish

1. Preview locally: `bundle exec jekyll serve`
2. Commit your changes: `git add . && git commit -m "Add new post"`
3. Push to GitHub: `git push origin main`

GitHub Pages will automatically build and deploy your site.

## 🎨 Customization

### Modifying Site Information

Edit `_config.yml` to update:
- Site title and description
- Social media links
- Author information
- Timezone
- Base URL

### Changing Colors and Styles

Edit `_sass/_variables.scss` to modify:
- Colors
- Fonts
- Spacing
- Breakpoints

### Adding New Projects

Edit `_data/projects.yml`:

```yaml
- name: Project Name
  description: Project description
  image: image-filename.svg
  github: https://github.com/username/repo
  demo: https://demo-url.com  # Optional
```

## 📝 Content Guidelines

### Blog Post Best Practices

- **Use descriptive titles**: Clear and engaging
- **Add excerpts**: Summarize posts in 1-2 sentences
- **Use headings**: Structure content with H2 and H3 tags
- **Include code blocks**: Format code properly with syntax highlighting
- **Add tags**: Help readers find related content
- **Proofread**: Check for typos and clarity

### Markdown Tips

- Use `##` for main headings, `###` for subheadings
- Wrap code in backticks: \`code\` for inline, \`\`\`language\`\`\` for blocks
- Create lists with `-` or `1.`
- Add links: `[text](url)`
- Insert images: `![alt text](image-url)`

## 🔧 Configuration

### Enabling Features

**RSS Feed**: Automatically generated at `/feed.xml`

**Sitemap**: Automatically generated at `/sitemap.xml`

**SEO Tags**: Automatically added to all pages

### Adding Plugins

Add new plugins to `Gemfile`:
```ruby
group :jekyll_plugins do
  gem "plugin-name"
end
```

Then run `bundle install` and add to `_config.yml`:
```yaml
plugins:
  - plugin-name
```

## 🚢 Deployment

This site is automatically deployed via GitHub Pages:

1. Push changes to the `main` branch
2. GitHub Actions builds the site
3. Changes go live at devwithdean.com

### Manual Build

To build the site manually:
```bash
bundle exec jekyll build
```

Output will be in the `_site/` directory.

## 🐛 Troubleshooting

### Common Issues

**Jekyll won't start**
- Ensure Ruby and Bundler are installed
- Run `bundle install` to install dependencies
- Check for port conflicts (default: 4000)

**Changes not showing**
- Hard refresh browser (Ctrl+Shift+R or Cmd+Shift+R)
- Clear Jekyll cache: `bundle exec jekyll clean`
- Restart development server

**Build errors on GitHub Pages**
- Check that all plugins are GitHub Pages compatible
- Verify YAML front matter syntax
- Review build logs in repository settings

## 📚 Resources

- [Jekyll Documentation](https://jekyllrb.com/docs/)
- [Markdown Guide](https://www.markdownguide.org/)
- [GitHub Pages Documentation](https://docs.github.com/en/pages)
- [Liquid Template Language](https://shopify.github.io/liquid/)

## 📄 License

This project is open source and available for personal use. Feel free to fork and customize for your own site!

## 👤 Author

**Dean**
- Website: [devwithdean.com](https://devwithdean.com)
- GitHub: [@DeanJ93](https://github.com/DeanJ93)
- Twitter: [@devwithdean](https://x.com/devwithdean)

## 🤝 Contributing

While this is a personal site, suggestions and feedback are welcome! Feel free to:
- Open an issue for bugs or suggestions
- Fork the repo for your own use
- Share your experience

## 📞 Contact

Have questions or want to connect? Reach out through:
- [Twitter](https://x.com/devwithdean)
- [GitHub](https://github.com/DeanJ93)
- [Instagram](https://www.instagram.com/devwithdean/)
- [Reddit](https://www.reddit.com/user/StomachExpert8659/)

---

**Happy Coding! 🚀**
