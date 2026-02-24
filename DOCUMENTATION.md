Manikandan P - Portfolio Website Documentation
📋 Project Overview
A modern, interactive portfolio website built with React, TypeScript, and Vite. Features a dark/light theme, custom cursor, particle animations, and smooth scroll interactions.

Live URL: [Your deployment URL]
Developer: Manikandan P
Tech Stack: React 19 + TypeScript + Vite + Framer Motion

🚀 Features
Core Features
Dual Theme System - Dark mode (default) and light mode with pixel-blast background

Custom Cursor - Interactive cursor with hover effects

Particle Background - Dynamic particle network with mouse interaction

Smooth Animations - Framer Motion powered scroll and interaction animations

Responsive Design - Mobile-first approach with hamburger menu

Type Animation - Dynamic typing effect for role titles

Contact Form - Functional contact form with backend integration

Sections
Hero - Introduction with animated avatar and social links

About - Personal info, education timeline, and stats

Skills - Categorized technical skills

Projects - 6 featured projects with tech stacks

Experience - Timeline-based work experience

Certifications - Professional certifications with download links

Contact - Contact form and information

🛠️ Tech Stack
Frontend
React 19.2.0 - UI library

TypeScript 5.9.3 - Type safety

Vite 7.3.1 - Build tool & dev server

Framer Motion 12.34.3 - Animations

Lucide React 0.575.0 - Icon library

React Type Animation 3.2.0 - Typing effects

Backend (Server)
Node.js + Express - Contact form API

Located in /server directory

Styling
Custom CSS - CSS variables for theming

Space Grotesk - Heading font

Inter - Body font

📁 Project Structure
Mani-Portfolio/
├── public/
│   ├── certificates/          # PDF certificates
│   └── resume.pdf            # Resume file
├── server/                   # Backend API
│   ├── index.js             # Express server
│   └── package.json
├── src/
│   ├── assets/              # Images
│   │   ├── profile.jpeg     # Dark theme avatar
│   │   ├── profile-light.jpg # Light theme avatar
│   │   └── pixel-blast.jpg  # Light theme background
│   ├── components/          # React components
│   │   ├── About.tsx        # About section
│   │   ├── Certifications.tsx
│   │   ├── Contact.tsx      # Contact form
│   │   ├── CustomCursor.tsx # Custom cursor
│   │   ├── Experience.tsx   # Work timeline
│   │   ├── Footer.tsx
│   │   ├── Hero.tsx         # Landing section
│   │   ├── Navbar.tsx       # Navigation
│   │   ├── ParticlesBackground.tsx
│   │   ├── Projects.tsx     # Project showcase
│   │   ├── Skills.tsx       # Skills grid
│   │   └── ThemeToggle.tsx  # Theme switcher
│   ├── context/
│   │   └── ThemeContext.tsx # Theme state management
│   ├── App.tsx              # Main app component
│   ├── index.css            # Global styles
│   └── main.tsx             # Entry point
├── package.json
├── tsconfig.json
└── vite.config.ts


Copy

Insert at cursor
🎨 Design System
Color Palette
Dark Theme:

Background: #050508 (primary), #0d0d12 (secondary)

Text: #ffffff (primary), #a0a0b0 (secondary)

Accent: #e5f22f (gold), #00d4ff (cyan)

Light Theme:

Background: #ffffff with pixel-blast image

Text: #111111 (primary), #444444 (secondary)

Accent: #b88746 (gold), #00aaff (cyan)

Typography
Headings: Space Grotesk (700-800 weight)

Body: Inter (400-600 weight)

🔧 Installation & Setup
Prerequisites
Node.js 18+ and npm

Installation
# Clone repository
git clone <repository-url>
cd Mani-Portfolio

# Install frontend dependencies
npm install

# Install backend dependencies
cd server
npm install
cd ..

Copy

Insert at cursor
Development
# Start frontend (port 5173)
npm run dev

# Start backend (port 5000) - in separate terminal
cd server
node index.js

Copy

Insert at cursor
bash
Build for Production
npm run build
npm run preview

Copy

Insert at cursor
bash
📦 Key Dependencies
Package	Version	Purpose
react	19.2.0	UI framework
framer-motion	12.34.3	Animations
lucide-react	0.575.0	Icons
react-type-animation	3.2.0	Typing effect
vite	7.3.1	Build tool
🎯 Component Architecture
Core Components
Hero.tsx

Landing section with avatar, typing animation, and CTA buttons

3D tilt effect on avatar with rotating glow rings

Social media links and download resume button

About.tsx

Personal introduction and education timeline

Interactive stat cards (Projects, CGPA, Certifications, Internships)

Contact information display

Projects.tsx

Grid layout of 6 featured projects

Tech stack badges and GitHub/live links

Hover effects with radial gradient

Skills.tsx

Categorized skill display (Frontend, Backend, Tools, Soft Skills)

Interactive skill tags

Experience.tsx

Timeline-based work experience

Alternating left/right layout

Certifications.tsx

Certificate cards with download links

Verified badges

Contact.tsx

Form with validation

Email integration via backend API

Utility Components
CustomCursor.tsx - Custom cursor with hover states
ParticlesBackground.tsx - Canvas-based particle network
ThemeToggle.tsx - Theme switcher button
Navbar.tsx - Sticky navigation with scroll effects

Context
ThemeContext.tsx - Global theme state (dark/light)

🎨 Animation System
Framer Motion Variants
fadeUp: { hidden: { opacity: 0, y: 40 }, visible: { opacity: 1, y: 0 } }
stagger: { visible: { transition: { staggerChildren: 0.12 } } }

Copy

Insert at cursor
typescript
Scroll Animations
useInView hook for viewport detection

Staggered children animations

Smooth transitions with cubic-bezier easing

🌐 Backend API
Endpoint: POST /send-email

Request Body:

{
  "name": "string",
  "email": "string",
  "subject": "string",
  "message": "string"
}

Copy

Insert at cursor
json
Response: 200 OK or error message

📱 Responsive Breakpoints
Desktop: > 1024px (full layout)

Tablet: 768px - 1024px (single column)

Mobile: < 768px (hamburger menu, simplified layout)

🎭 Theme System
Toggle between dark and light themes using the sun/moon icon in the navbar.

Implementation:

Context API for global state

CSS variables for dynamic theming

LocalStorage persistence

Smooth transitions between themes

🚀 Deployment
Build Output
npm run build  # Creates /dist folder

Copy

Insert at cursor
bash
Hosting Options
Vercel - Recommended (zero config)

Netlify - Easy deployment

AWS S3 + CloudFront - Scalable solution

Environment Variables
Configure backend API URL in production build.

📝 Customization Guide
Update Personal Info
Edit data in respective component files:

Hero.tsx - Name, roles, social links

About.tsx - Bio, education, contact

Projects.tsx - Project list

Skills.tsx - Skill categories

Experience.tsx - Work history

Certifications.tsx - Certificates

Change Colors
Modify CSS variables in index.css:

:root {
  --accent-gold: #e5f22f;
  --bg-primary: #050508;
  /* ... */
}

Copy

Insert at cursor
css
Add New Sections
Create component in /src/components

Import in App.tsx

Add navigation link in Navbar.tsx

🐛 Known Issues & Solutions
Issue: Profile image not loading
Solution: Ensure profile.jpeg exists in /src/assets

Issue: Contact form not working
Solution: Start backend server on port 5000

Issue: Cursor not visible on mobile
Solution: Intentional - hidden via CSS media query

📄 License
Personal portfolio project - All rights reserved.

👤 Contact
Manikandan P
📧 mailto:manikandantamil42@gmail.com
📱 +91 6382392759
🎓 K.S.Rangasamy College of Technology

🔮 Future Enhancements
 Blog section with MDX support
 Project filtering by technology
 Dark mode toggle animation improvements
 Performance optimization (lazy loading)
 SEO meta tags and Open Graph
 Analytics integration
 Testimonials section