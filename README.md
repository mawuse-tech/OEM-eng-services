# OEM Engineering Services website

Responsive React and Vite website for OEM Engineering Services, a technical provider of vehicle accident inspections, damage assessments and reporting support for motor claims.

## Run locally

```sh
npm install
npm run dev
```

Create a production bundle with `npm run build`; preview it with `npm run preview`. `npm run lint` runs ESLint.

The project uses the React and Vite dependencies already present in the starter workspace. Additional dependency installation was unavailable in the build environment, so navigation and icons are implemented with browser history, React and CSS rather than third-party router/icon packages. Styling is authored in `src/App.css` and `src/index.css`.

## Content to verify before launch

- Replace contact placeholders in the footer and contact page with verified company phone, email and office details.
- Confirm service availability and scope, especially repair scope and cost assessment.
- Review and approve the proposed mission and vision wording on the About page.
- Review and approve the draft Privacy Policy with the company’s actual information handling and retention practices.
- Replace temporary Unsplash automotive images and temporary wordmark with OEM-owned/approved imagery and the official logo. Image URLs and descriptions are in `src/App.jsx`.
- Connect the Contact form in `src/App.jsx` to an approved backend or email service. The current form performs client-side validation and displays a development-only message; it does not transmit or retain submitted information.

## Structure

- `src/App.jsx` contains the page components, shared layout, navigation, content data and form behavior.
- `src/App.css` contains the responsive visual system and component styles.
- `src/index.css` contains global styles and design tokens.
- `index.html` contains base SEO and social sharing metadata.

## Deployment

Run `npm run build` and deploy the generated `dist/` directory to a static host. Configure the host to serve `index.html` for application routes such as `/services` and `/privacy`.

The current image URLs require network access. For production, use appropriately licensed optimized local images. Add a canonical domain, production social sharing image, robots policy and sitemap after the deployment URL is confirmed.
