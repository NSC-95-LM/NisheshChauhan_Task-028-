# NisheshChauhan_Task(28)

A creative digital marketplace web application built with **React 19**, **Vite**, **Tailwind CSS v4**, and **React Router DOM v7**.

---

## Summary

This project showcases a complete multi-page Single Page Application (SPA) structured around a modern creative marketplace (NSC). The primary objective of this task is to demonstrate an advanced understanding and implementation of **React Router DOM**, featuring:
- Centralized nested routing architecture with `<Outlet />` and `<Layout />`.
- Modern data-router patterns using `createBrowserRouter` and `createRoutesFromElements`.
- Active link tracking and dynamic styling with `<NavLink>`.
- Cross-route hash navigation with automatic smooth scrolling.
- Programmatic navigation via `useNavigate()`.
- Global automatic scroll-to-top on route changes.
- Wildcard 404 error handling for broken or unmapped paths.

---

## What it Does?

The platform connects digital creators (brand designers, illustrators, UI/UX engineers) with buyers looking for high-quality digital assets:
1. **Home (`/`)**:
   - **Hero Section:** Features floating animated product price badges (`UI Kit`, `Logo Pack`, `Templates`).
   - **Stats Section:** Key platform community metrics.
   - **Explore Categories:** Interactive cards highlighting asset categories.
   - **Meet Our Creators:** Featured artist profiles with ratings and product catalogs.
   - **Trending Products:** Product showcase cards with prices, ratings, and call-to-actions.
   - **How It Works:** Dedicated 3-step flows for both Creators and Buyers.
   - **Testimonials & Final CTA:** Customer and seller reviews with direct conversion buttons.
2. **About Us (`/about`)**:
   - Company mission and vision for empowering digital creators.
   - Core value propositions (Creativity, Trust & Security, Community).
   - Founding leadership team showcase.
3. **Contact Us (`/contact`)**:
   - Direct support channels (Email, Phone, Headquarters, Response time SLA).
   - Interactive contact inquiry form with controlled state and submission feedback.
4. **Login (`/login`)**:
   - Clean, centered authentication card with email/password inputs, remember me option, and redirection logic.
5. **Signup (`/signup`)**:
   - Onboarding form with role switching (**Creator / Seller** vs. **Buyer / Agency**) and terms agreement.
6. **404 Not Found (`*`)**:
   - Custom catch-all page with options to return home or go back via history stack (`navigate(-1)`).
7. **Cross-Page Section Navigation & Scroll Restoration**:
   - Footer section links (`/#categories`, `/#creators`, etc.) seamlessly switch from any route back to the home page and smoothly scroll to the exact target section.
   - Navigating between standard pages automatically scrolls the viewport smoothly back to the top.

---

## Project Structure

```
nsc-28-vite/
├── public/
│   └── favicon.ico
├── src/
│   ├── assets/               # Product images and creator avatars
│   ├── components/
│   │   ├── about/            # About page component
│   │   ├── common/           # Common utilities (ScrollToTop.jsx)
│   │   ├── contact/          # Contact page component & form
│   │   ├── footer/           # Persistent footer with navigation links
│   │   ├── header/           # Persistent sticky navigation header
│   │   ├── home/             # Home page with marketplace sections
│   │   ├── login/            # Centered login component
│   │   ├── notFound/         # Custom 404 page component
│   │   ├── signup/           # Centered signup component with role picker
│   │   └── Index.jsx         # Component barrel export
│   ├── hoc/
│   │   └── Layout.jsx        # Root Layout wrapping Header, Outlet, Footer, ScrollToTop
│   ├── input.css             # Tailwind CSS imports
│   ├── main.jsx              # Router configuration and application entry point
│   └── App.jsx
├── index.html                # HTML entry with font imports & AOS script
├── package.json              # Project dependencies and npm scripts
└── vite.config.js            # Vite configuration with React & Tailwind plugins
```

---

## How to Run?

### 1. Prerequisites
Ensure you have [Node.js](https://nodejs.org/) installed (version 18+ recommended).

### 2. Installation
Open your terminal inside the project directory:
```bash
cd nsc-28-vite
npm install
```

### 3. Start Development Server
```bash
npm run dev
```
Open your browser and navigate to the local URL (usually `http://localhost:5173`).

### 4. Build for Production
```bash
npm run build
```

### 5. Preview Production Build
```bash
npm run preview
```

---

## Technologies Used

- **React 19** - Front-end component library
- **React Router DOM v7** - Client-side routing, navigation, layout management, and history handling
- **Vite** - Next-generation frontend build tooling
- **Tailwind CSS v4** - Utility-first styling with custom palette
- **Ionicons** - Vector icon set for UI elements and social icons
- **AOS (Animate On Scroll)** - Scroll animations for creator cards

---

## Author

**Nishesh Chauhan**  
*Task 28 Submission*