# Blog - Next.js Personal Blog

A modern, responsive personal blog built with Next.js featuring markdown-based content management, static site generation, and a clean, professional design.

## 🚀 Features

- **Static Site Generation (SSG)** - Fast loading with pre-rendered pages
- **Markdown-based Content** - Write blog posts in markdown with frontmatter metadata
- **Responsive Design** - Mobile-first approach with CSS modules
- **Syntax Highlighting** - Code blocks with syntax highlighting using Prism
- **Image Optimization** - Next.js Image component for optimized images
- **File-based Routing** - Automatic routing based on file structure
- **Contact Form** - Simple contact form for user interaction
- **Featured Posts** - Highlight important posts on the homepage

## 🛠️ Tech Stack

- **Framework**: Next.js 13.2.4
- **React**: 18.2.0
- **Styling**: CSS Modules
- **Content**: Markdown with gray-matter
- **Syntax Highlighting**: react-syntax-highlighter
- **Markdown Rendering**: react-markdown

## 📁 Project Structure

```
Blog/
├── components/           # Reusable React components
│   ├── contact/         # Contact form components
│   ├── home-page/       # Homepage specific components
│   ├── layout/          # Layout and navigation components
│   └── posts/           # Post-related components
├── lib/                 # Utility functions
│   └── posts-util.js    # Post data processing utilities
├── pages/               # Next.js pages (file-based routing)
│   ├── posts/           # Blog posts pages
│   ├── _app.js          # App wrapper
│   ├── contact.js       # Contact page
│   └── index.js         # Homepage
├── posts/               # Markdown blog posts
├── public/              # Static assets
│   └── images/          # Images for posts and site
└── styles/              # Global styles
    └── globals.css      # Global CSS variables and styles
```

## 🚀 Getting Started

### Prerequisites

- Node.js 14+ 
- npm or yarn

### Installation

1. Clone the repository:
```bash
git clone <repository-url>
cd Blog
```

2. Install dependencies:
```bash
npm install
# or
yarn install
```

3. Run the development server:
```bash
npm install
# and
npm run dev
# or
yarn dev
```

4. Open [http://localhost:3000](http://localhost:3000) in your browser.

## 📝 Adding New Blog Posts

1. Create a new markdown file in the `posts/` directory
2. Add frontmatter metadata at the top:

```markdown
---
title: 'Your Post Title'
date: '2023-01-01'
image: your-image.png
excerpt: 'Brief description of your post'
isFeatured: true
---

Your post content here...
```

3. Add any images to `public/images/posts/[slug]/`
4. The post will automatically appear in your blog

## 🎨 Customization

### Styling
- Global styles are in `styles/globals.css`
- Component-specific styles use CSS Modules
- Color scheme and typography can be customized via CSS variables

### Content
- Update the hero section in `components/home-page/hero.js`
- Modify navigation in `components/layout/main-navigation.js`
- Customize the contact form in `components/contact/contact-form.js`

## 📱 Pages

- **Homepage** (`/`) - Features hero section and featured posts
- **All Posts** (`/posts`) - Complete list of all blog posts
- **Individual Post** (`/posts/[slug]`) - Full post content with syntax highlighting
- **Contact** (`/contact`) - Contact form for user inquiries

## 🔧 Available Scripts

- `npm run dev` - Start development server
- `npm run build` - Build for production
- `npm run start` - Start production server
- `npm run lint` - Run ESLint

## 📦 Dependencies

### Production
- `next` - React framework
- `react` & `react-dom` - UI library
- `gray-matter` - Parse markdown frontmatter
- `react-markdown` - Render markdown content
- `react-syntax-highlighter` - Syntax highlighting

### Development
- `eslint` - Code linting
- `eslint-config-next` - Next.js ESLint configuration

## 🌟 Key Features Explained

### Static Site Generation
The blog uses Next.js SSG for optimal performance:
- Posts are pre-rendered at build time
- Fast loading and SEO-friendly
- Automatic revalidation for content updates

### Markdown Processing
- Posts are written in markdown with YAML frontmatter
- Automatic parsing and metadata extraction
- Support for images, code blocks, and rich formatting

### Responsive Design
- Mobile-first CSS approach
- Flexible grid layouts
- Optimized images with Next.js Image component

## 🚀 Deployment

The blog can be deployed to any platform that supports Next.js:

- **Vercel** (recommended)
- **Netlify**
- **AWS Amplify**
- **Traditional hosting** with Node.js support

**Built with**: Next.js, React, and lots of ☕
