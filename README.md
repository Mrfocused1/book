# Bood - Nature's Purest Ritual

A modern, elegant website for Bood - showcasing wildcrafted sea moss and adaptogenic mushrooms for holistic wellness.

## Features

- **Responsive Design**: Fully mobile-optimized with Tailwind CSS
- **Smooth Animations**: GSAP ScrollTrigger animations throughout
- **Modern UI**: Clean, elegant design with mix-blend modes and parallax effects
- **Fast Loading**: Optimized performance with Lenis smooth scrolling

## Pages

- **Home** (`index.html`) - Hero section, manifesto, visual storytelling, collection preview
- **Collection** (`collection.html`) - Product catalog with filters
- **Guide** (`guide.html`) - Daily ritual guide with recipes
- **Learn** (`learn.html`) - Educational compendium about sea moss
- **Lion's Mane** (`lions-mane.html`) - Product page for Lion's Mane mushrooms
- **Contact** (`contact.html`) - Contact form and FAQ

## Technologies

- **HTML5** - Semantic markup
- **Tailwind CSS** - Utility-first styling
- **GSAP** - Advanced animations
- **Lenis** - Smooth scrolling
- **Vercel** - Deployment platform

## Local Development

1. Clone the repository:
```bash
git clone https://github.com/yourusername/bood-website.git
cd bood-website
```

2. Start a local server:
```bash
python3 -m http.server 8000
# or
npm run dev
```

3. Open your browser:
```
http://localhost:8000
```

## Deployment to Vercel

### Option 1: Deploy via Vercel CLI

1. Install Vercel CLI:
```bash
npm i -g vercel
```

2. Deploy:
```bash
vercel
```

### Option 2: Deploy via GitHub

1. Push your code to GitHub:
```bash
git init
git add .
git commit -m "Initial commit"
git branch -M main
git remote add origin https://github.com/yourusername/bood-website.git
git push -u origin main
```

2. Go to [vercel.com](https://vercel.com)
3. Click "Add New Project"
4. Import your GitHub repository
5. Click "Deploy"

Your site will be live at `https://your-project-name.vercel.app`

## Project Structure

```
bood-website/
├── index.html           # Homepage
├── collection.html      # Products page
├── guide.html          # Daily guide page
├── learn.html          # Educational content
├── lions-mane.html     # Lion's Mane product page
├── contact.html        # Contact page
├── boodd.png          # Brand asset
├── package.json       # Project metadata
├── vercel.json        # Vercel configuration
├── .gitignore         # Git ignore rules
└── README.md          # This file
```

## Color Palette

- **Moss** - `#1a2e2a` (Dark green)
- **Sand** - `#e8e6e1` (Light beige)
- **Clay** - `#bfafa6` (Medium beige)
- **Gold** - `#d4af37` (Accent gold)
- **Ocean** - `#2b4c4a` (Deep teal)

## Typography

- **Serif** - Playfair Display (Headings, italic accent text)
- **Sans** - Manrope (Body text, navigation)

## Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)

## Performance

- Lighthouse Score: 90+
- Mobile-optimized
- Lazy-loaded animations
- Optimized images

## License

MIT License - feel free to use this project as inspiration for your own work.

## Contact

For questions or support, visit [contact page](https://your-domain.com/contact.html)
