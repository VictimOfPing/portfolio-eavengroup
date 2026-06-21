# Eaven Group

![Next.js](https://img.shields.io/badge/Next.js-16.1.3-black?style=for-the-badge&logo=nextdotjs)
![React](https://img.shields.io/badge/React-19.2.3-61DAFB?style=for-the-badge&logo=react&logoColor=111111)
![TypeScript](https://img.shields.io/badge/TypeScript-5.x-3178C6?style=for-the-badge&logo=typescript&logoColor=ffffff)
![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-4.x-06B6D4?style=for-the-badge&logo=tailwindcss&logoColor=ffffff)
![Framer Motion](https://img.shields.io/badge/Framer_Motion-12.x-0055FF?style=for-the-badge&logo=framer&logoColor=ffffff)

Eaven Group needed a polished digital presence for a premium real estate management brand focused on selected luxury assets in Italy.  
This project delivers a fast, responsive corporate website with cinematic property imagery, service storytelling, SEO-ready metadata, and a direct contact flow for private consultations.

**Live site:** [eavengroup.com](https://eavengroup.com)  
**Industry:** Luxury real estate and property management

## Preview

The repository does not include a captured browser screenshot. The brand asset below is included in the project and the complete interface can be reviewed on the live deployment.

<p align="center">
  <a href="https://eavengroup.com">
    <img src="./public/logo.png" alt="Eaven Group logo" width="280" />
  </a>
</p>

## Tech Stack

| Layer | Tools |
| --- | --- |
| Framework | ![Next.js](https://img.shields.io/badge/Next.js-16.1.3-black?logo=nextdotjs) |
| UI | ![React](https://img.shields.io/badge/React-19.2.3-61DAFB?logo=react&logoColor=111111) ![TypeScript](https://img.shields.io/badge/TypeScript-5.x-3178C6?logo=typescript&logoColor=ffffff) |
| Styling | ![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-4.x-06B6D4?logo=tailwindcss&logoColor=ffffff) ![shadcn/ui](https://img.shields.io/badge/shadcn%2Fui-New_York-111111) |
| Motion and icons | ![Framer Motion](https://img.shields.io/badge/Framer_Motion-12.x-0055FF?logo=framer&logoColor=ffffff) ![Lucide](https://img.shields.io/badge/Lucide_React-0.562-F56565) |
| Validation and SEO | ![Zod](https://img.shields.io/badge/Zod-4.x-3068B7) Next.js Metadata API, sitemap, robots, web manifest |

## Main Features

- Animated full-screen hero with rotating luxury property imagery and slide indicators.
- Responsive corporate navigation with desktop links, mobile full-screen menu, and scroll-aware brand treatment.
- Dedicated content pages for company positioning, services, and contact conversion.
- Client-side contact form with Zod validation, request categorization, loading state, and success/error feedback.
- SEO foundation with structured metadata, Open Graph image generation, sitemap, robots configuration, favicon, and app icons.

## Project Structure

The project uses the Next.js App Router with a clear separation between route-level pages, shared layout, reusable components, and small configuration modules.

```text
src/
  app/
    page.tsx                 Home route composition
    layout.tsx               Global metadata, fonts, navbar, footer
    chi-siamo/               About page route
    cosa-facciamo/           Services page route
    contatti/                Contact page route
    sitemap.ts               Dynamic sitemap generation
    robots.ts                Search crawler rules
    manifest.ts              Web app manifest
  components/
    hero.tsx                 Animated homepage hero
    navbar.tsx               Responsive site navigation
    contact-form.tsx         Validated enquiry form
    cta-section.tsx          Conversion section
    ui/                      shadcn-style primitives
  lib/
    site.ts                  Site name, locale, canonical URL, description
    company.ts               Company-level constants
```

Remote Unsplash imagery is explicitly allowed in `next.config.ts`, while brand identity, icons, and manifest assets live under `public/`.

## Results and Impact

- Replaced the default starter experience with a production-oriented brand website for Eaven Group.
- Turned a service-led positioning into a structured user journey: homepage, credibility content, service detail, and consultation request.
- Added technical SEO essentials so the site can expose canonical routes, social previews, sitemap data, and crawl rules from the app itself.
- Kept the stack lean and maintainable: no CMS or backend dependency is required for the current brochure and lead-capture scope.

## Run Locally

```bash
npm install
npm run dev
```

Open `http://localhost:3000` to view the site.

Useful commands:

```bash
npm run lint
npm run build
npm run start
```

## Contact and Portfolio

- Live project: [https://eavengroup.com](https://eavengroup.com)
- Client contact: [info@EavenGroup.com](mailto:info@EavenGroup.com)
- Instagram: [@eavengroup](https://instagram.com/eavengroup)
- Developer portfolio / source profile: [VictimOfPing on GitHub](https://github.com/VictimOfPing)
