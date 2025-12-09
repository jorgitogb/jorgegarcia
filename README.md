# Jorge Garcia Brizuela - Personal Landing Page

A modern, professional personal landing page built with Astro and Tailwind CSS, showcasing professional profile and GitHub projects.

## 🚀 Features

- **Modern Design**: Glassmorphism effects, smooth animations, and gradient accents
- **Responsive**: Fully responsive design that works on all devices
- **Dynamic Content**: Automatically fetches and displays GitHub repositories
- **SEO Optimized**: Proper meta tags and semantic HTML
- **Fast Performance**: Built with Astro for optimal performance
- **Social Links**: Direct links to GitHub, LinkedIn, and ORCID profiles

## 🛠️ Tech Stack

- **Astro** - Static site generator
- **Tailwind CSS v4** - Utility-first CSS framework
- **TypeScript** - Type-safe development
- **GitHub API** - Dynamic project showcase

## 📦 Installation

```bash
# Install dependencies
npm install

# Start development server
npm run dev

# Build for production
npm run build

# Preview production build
npm run preview
```

## 🌐 Deployment to Cloudflare Pages

### Option 1: Using Cloudflare Dashboard

1. **Build your site locally**:
   ```bash
   npm run build
   ```

2. **Push to GitHub**:
   ```bash
   git add .
   git commit -m "Initial commit"
   git push origin main
   ```

3. **Deploy to Cloudflare Pages**:
   - Go to [Cloudflare Dashboard](https://dash.cloudflare.com/)
   - Navigate to **Pages** → **Create a project**
   - Connect your GitHub repository
   - Configure build settings:
     - **Build command**: `npm run build`
     - **Build output directory**: `dist`
     - **Environment variables**: None required
   - Click **Save and Deploy**

### Option 2: Using Wrangler CLI

```bash
# Install Wrangler
npm install -g wrangler

# Login to Cloudflare
wrangler login

# Deploy
npm run build
wrangler pages deploy dist
```

## 📝 Customization

### Update Personal Information

Edit `src/pages/index.astro`:
- Change the GitHub username in the fetch URL
- Update social links
- Modify hero section text

### Customize Colors

Edit `src/styles/global.css`:
- Modify CSS variables in `:root`
- Adjust gradient colors
- Change animation timings

### Add More Sections

Create new components in `src/components/` and import them into `index.astro`.

## 📄 Project Structure

```
/
├── public/
│   └── favicon.svg
├── src/
│   ├── components/
│   │   ├── ProjectCard.astro
│   │   └── SocialLink.astro
│   ├── layouts/
│   │   └── Layout.astro
│   ├── pages/
│   │   └── index.astro
│   └── styles/
│       └── global.css
├── astro.config.mjs
├── package.json
└── tsconfig.json
```

## 🎨 Design Features

- **Glassmorphism**: Frosted glass effect on cards and links
- **Smooth Animations**: Fade-in, float, and glow effects
- **Gradient Text**: Eye-catching gradient on name
- **Hover Effects**: Interactive hover states on all clickable elements
- **Dark Theme**: Modern dark color scheme with vibrant accents

## 📱 Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)

## 📧 Contact

- **GitHub**: [jorgitogb](https://github.com/jorgitogb)
- **LinkedIn**: [jorge-garcia-brizuela-b56669aa](https://www.linkedin.com/in/jorge-garcia-brizuela-b56669aa/)
- **ORCID**: [0000-0003-0527-1339](https://orcid.org/0000-0003-0527-1339)

## 📄 License

MIT License - feel free to use this template for your own personal website!

---

Built with ❤️ using Astro and Tailwind CSS
