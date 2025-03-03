
# Socially
<div align="center">
  <img src="public/socially-logo.svg" alt="Socially Logo" width="200" height="50"/>
  <h3>A modern social platform for connecting with friends and sharing your world</h3>
</div>

## ✨ Features

- **User Authentication**: Secure sign-up and login using Clerk
- **Responsive Design**: Beautiful UI that works on both mobile and desktop
- **Dark/Light Modes**: Choose your preferred theme
- **Real-time Updates**: Instant notifications and content refreshing
- **Media Uploads**: Share images and media with UploadThing integration
- **Interactive UI**: Modern interface with subtle animations and transitions
- **PostgreSQL Database**: Robust data storage with Neon PostgreSQL

## 🛠️ Tech Stack

- **Frontend**: Next.js 14, React, Tailwind CSS
- **Authentication**: Clerk
- **Database**: PostgreSQL (Neon)
- **Styling**: Tailwind CSS with custom components
- **Fonts**: Outfit (headlines), Geist Sans (body), Geist Mono (code)
- **File Uploads**: UploadThing
- **State Management**: React Context API
- **Deployment**: Vercel

## 🚀 Getting Started

### Prerequisites

- Node.js 18.x or later
- npm or yarn
- Git

### Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/ft-prince/Socially.git
   cd socially
   ```

2. Install dependencies:
   ```bash
   npm install
   # or
   yarn install
   ```

3. Set up environment variables (create a `.env.local` file in the root directory):
   ```
   # Clerk Authentication (get from https://clerk.dev)
   NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY=your_publishable_key
   CLERK_SECRET_KEY=your_secret_key

   # PostgreSQL Database (Neon)
   DATABASE_URL=your_database_url

   # UploadThing
   UPLOADTHING_TOKEN=your_uploadthing_token
   ```

4. Run the development server:
   ```bash
   npm run dev
   # or
   yarn dev
   ```

5. Open [http://localhost:3000](http://localhost:3000) in your browser to see the application.

## 📦 Project Structure

```
socially/
├── app/              # Next.js app directory
├── components/       # React components
│   ├── Navbar.tsx    # Modern navigation bar
│   ├── Sidebar.tsx   # Application sidebar
│   └── ...
├── lib/              # Utility functions and shared code
├── prisma/           # Database schema and migrations
├── public/           # Static assets
└── styles/           # Global styles and Tailwind configuration
```

## 🔒 Environment Variables

This project requires several environment variables to function correctly:

- **Clerk Authentication**:
  - `NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY`: Public key for Clerk frontend auth
  - `CLERK_SECRET_KEY`: Secret key for Clerk server-side auth

- **Database**:
  - `DATABASE_URL`: PostgreSQL connection string (Neon)

- **File Uploads**:
  - `UPLOADTHING_TOKEN`: API token for UploadThing service

> ⚠️ **Important**: Never commit your actual .env files to version control. The `.env.local` file should be added to `.gitignore`.

## 🎨 Styling System

Socially uses a three-tier font system:

- **Headlines/Brand**: Outfit font (Google Fonts)
- **Body Text**: Geist Sans for clean, readable content
- **Code/Monospace**: Geist Mono for technical elements

Custom utility classes:
- `gradient-text`: Gradient text for branding elements
- `hero-text`: Bold, impactful headlines
- `brand-name`: Distinctive styling for the brand
- `caption-text`: Styled smaller text elements

## 🧩 Components

### Modern Navbar

The application features a sleek, responsive navbar with:
- Gradient text branding
- Custom SVG icon
- Smooth hover animations
- Full mobile responsiveness
- Dark/light mode support

### Content Layout

The main content area is structured with:
- Responsive grid system
- Sidebar (desktop only)
- Content area with proper spacing
- Subtle background gradients for depth

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

1. Fork the project
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the MIT License - see the LICENSE file for details.

## 🙏 Acknowledgements

- [Next.js](https://nextjs.org/)
- [Clerk](https://clerk.dev/)
- [Neon PostgreSQL](https://neon.tech/)
- [Tailwind CSS](https://tailwindcss.com/)
- [Geist Font](https://vercel.com/font)
- [Outfit Font](https://fonts.google.com/specimen/Outfit)
- [UploadThing](https://uploadthing.com/)
