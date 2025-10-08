# Berkay Aktunç - Personal Blog

A multilingual personal blog built with Hugo and the KeepIt theme, supporting both English and Turkish.

## 🌐 Languages

- **English** (Primary) - `/`
- **Turkish** - `/tr/`

## 🚀 Features

- **Multilingual Support**: English and Turkish
- **Responsive Design**: Works on all devices
- **Modern Theme**: KeepIt theme with customizations
- **SEO Optimized**: Meta tags and structured data
- **Fast Loading**: Static site generation with Hugo
- **GitHub Pages Ready**: Automatic deployment

## 📁 Content Structure

```
content/
├── _index.md          # English homepage
├── about.md           # English about page
├── posts/             # English blog posts
│   └── welcome.md
└── tr/                # Turkish content
    ├── _index.md      # Turkish homepage
    ├── about.md       # Turkish about page
    └── posts/         # Turkish blog posts
        └── first.md
```

## 🛠️ Development

### Prerequisites

- Hugo Extended (v0.150.1 or later)
- Git

### Local Development

1. Clone the repository:
   ```bash
   git clone https://github.com/berkayaktunc/berkayaktunc.github.io.git
   cd berkayaktunc.github.io
   ```

2. Start the development server:
   ```bash
   hugo server --buildDrafts --buildFuture
   ```

3. Open your browser and go to `http://localhost:1313`

### Building for Production

```bash
hugo --buildDrafts --buildFuture
```

## 📝 Adding New Content

### English Content

Create new posts in `content/posts/`:
```bash
hugo new posts/my-new-post.md
```

### Turkish Content

Create new posts in `content/tr/posts/`:
```bash
hugo new tr/posts/yeni-yazim.md
```

### Front Matter

Each post should include proper front matter:

```yaml
+++
title = "Post Title"
date = 2024-01-01T00:00:00+03:00
draft = false
author = "Berkay Aktunç"
description = "Post description"
tags = ["tag1", "tag2"]
categories = ["category"]
+++
```

## 🎨 Customization

### Site Configuration

Edit `hugo.toml` to customize:
- Site title and description
- Social media links
- Theme settings
- Language settings

### Adding New Languages

1. Add language configuration in `hugo.toml`:
   ```toml
   [languages.fr]
     languageName = "Français"
     weight = 3
     title = "Berkay Aktunç"
     description = "Développeur de logiciels et passionné de technologie"
   ```

2. Create content directory:
   ```bash
   mkdir -p content/fr/posts
   ```

3. Add menu configuration for the new language

## 🚀 Deployment

This site is automatically deployed to GitHub Pages using GitHub Actions. Simply push to the `main` branch and the site will be built and deployed automatically.

### Manual Deployment

1. Build the site:
   ```bash
   hugo --buildDrafts --buildFuture
   ```

2. The `public/` directory contains the static files ready for deployment.

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

## 🤝 Contributing

Feel free to submit issues and enhancement requests!

## 📞 Contact

- **Email**: [email@example.com](mailto:email@example.com)
- **GitHub**: [@berkayaktunc](https://github.com/berkayaktunc)
- **LinkedIn**: [Berkay Aktunç](https://linkedin.com/in/berkayaktunc)

---

Made with ❤️ using [Hugo](https://gohugo.io/) and [KeepIt](https://github.com/Fastbyte01/KeepIt) theme.
