# 🌟 GreyBeez Website

> Empowering rural and tribal youth with market-ready skills through comprehensive training programs and direct placement with leading manufacturers.

## 🚀 Features

- **Hero Section**: Dynamic carousel controlled through Strapi CMS
- **Partner Logos**: Colorful brand partner logos with infinite scroll carousel
- **Impact Highlights**: Statistics and success metrics
- **Program Spotlight**: Training programs showcase
- **Services Snapshot**: Service offerings overview
- **Testimonials**: Success stories and feedback
- **Multilingual Support**: English, Hindi, Bengali, and Oriya
- **Responsive Design**: Mobile-first approach with Tailwind CSS

## 🛠️ Tech Stack

- **Frontend**: React 18 + TypeScript + Vite
- **Styling**: Tailwind CSS
- **CMS**: Strapi (Headless CMS)
- **Internationalization**: react-i18next
- **Deployment**: Vercel
- **Package Manager**: npm

## 📁 Project Structure

```
src/
├── components/          # React components
│   ├── HeroCarousel.tsx        # Strapi-controlled hero section
│   ├── PartnerLogosCarousel.tsx # Brand partner logos
│   ├── ImpactHighlights.tsx    # Statistics display
│   ├── ProgramSpotlight.tsx    # Programs showcase
│   ├── ServicesSnapshot.tsx    # Services overview
│   ├── Testimonials.tsx        # Success stories
│   └── FinalCTA.tsx            # Call-to-action
├── services/            # API services
│   └── strapiService.ts # Strapi integration
├── config/              # Configuration files
│   └── strapi.ts        # Strapi settings
├── i18n.ts             # Internationalization setup
└── main.tsx            # Application entry point
```

## 🎯 Strapi Integration

### Hero Section
- **Content Type**: `homepage-heroslide`
- **Fields**: Title, HeroImage, DisplayOrder, isActive
- **API Endpoint**: `/api/homepage-heroslides`

### Partner Logos
- **Content Type**: `brand-partner-logo`
- **Fields**: companyname, logo, order, isActive
- **API Endpoint**: `/api/brand-partner-logos`

## 🚀 Getting Started

### Prerequisites
- Node.js 18+ 
- npm or yarn
- Strapi instance running

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/CTOatgreybeez/greybeez-website.git
   cd greybeez-website
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Configure Strapi**
   - Update `src/config/strapi.ts` with your Strapi URL
   - Set up content types as documented

4. **Start development server**
   ```bash
   npm run dev
   ```

5. **Build for production**
   ```bash
   npm run build
   ```

## 🌐 Environment Configuration

Create a `.env` file in the root directory:

```env
VITE_STRAPI_URL=http://localhost:1337
VITE_STRAPI_API_URL=http://localhost:1337/api
```

## 📱 Available Scripts

- `npm run dev` - Start development server
- `npm run build` - Build for production
- `npm run preview` - Preview production build
- `npm run lint` - Run ESLint
- `npm run type-check` - Run TypeScript type checking

## 🎨 Customization

### Adding New Sections
1. Create component in `src/components/`
2. Import and add to `src/App.tsx`
3. Update routing if needed

### Strapi Content Types
1. Create content type in Strapi admin
2. Add service method in `strapiService.ts`
3. Update component to use Strapi data

## 🌍 Internationalization

The website supports multiple languages:
- **English (en)** - Default
- **Hindi (hi)**
- **Bengali (bn)**
- **Oriya (or)**

Translation files are located in `public/locales/`.

## 🚀 Deployment

### Vercel (Recommended)
1. Connect your GitHub repository to Vercel
2. Set environment variables
3. Deploy automatically on push to main branch

### Manual Deployment
1. Build the project: `npm run build`
2. Upload `dist/` folder to your hosting provider

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch: `git checkout -b feature/amazing-feature`
3. Commit changes: `git commit -m 'Add amazing feature'`
4. Push to branch: `git push origin feature/amazing-feature`
5. Open a Pull Request

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🆘 Support

For support and questions:
- Create an issue in this repository
- Contact the development team
- Check the [Strapi documentation](https://docs.strapi.io/)

## 🙏 Acknowledgments

- Strapi team for the excellent headless CMS
- Tailwind CSS for the utility-first CSS framework
- React team for the amazing frontend library
- All contributors and supporters of GreyBeez

---

**Built with ❤️ for empowering rural and tribal youth**