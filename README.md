# Rumble Cars 🚗

A modern car rental website built with React.js, featuring an intuitive interface for browsing 
and renting vehicles from various car brands.

## 📋 Table of Contents

- Home
- Features
- Project Structure
- Pages Overview
- Installation
- Usage
- Technologies Used
- Component Architecture
- Routing System
- Screenshots
- Learning Outcomes
- Future Enhancements
- Contributing
- Authors
- License

### 🎯 About
Rumble Cars is my first React.js project - a comprehensive car rental platform that showcases modern web development practices. This project represents my journey in learning React fundamentals, component-based architecture, and client-side routing.
The platform allows users to:

- Browse through various car brands (marques)
- View detailed car models for each brand
- Learn about the company and its services
- Read automotive blog posts
- Contact the rental service

This project served as a practical learning experience for understanding:

- React component lifecycle
- React Router for navigation
- Component reusability and props
- State management
- Modern JavaScript (ES6+)

### ✨ Features
Core Features :

- 🏠 Dynamic Homepage: Welcoming landing page with featured cars
- 🚘 Brand Catalog: Comprehensive list of car manufacturers
- 🔍 Model Browser: Detailed view of car models by brand
- 📝 Blog Section: Automotive articles and news
- 💼 Services Page: Detailed rental services and packages
- 📞 Contact Form: Easy communication channel
- ℹ️ About Us: Company information and mission
- 🧭 Responsive Navigation: Smooth routing between pages

Technical Features :

- ⚛️ Component-based architecture
- 🛣️ React Router implementation
- 📱 Responsive design
- 🎨 Modern UI/UX
- ⚡ Fast page transitions
- 🔄 Reusable components

### 📁 Project Structure
```
rumble-cars/
├── public/
│   ├── index.html
│   └── images/
│       ├── logo.png
├── src/
│   ├── components/          # There is a lot of components here  
│   ├── pages/                
│   │   ├── Home/
│   │   │   ├── Home.jsx
│   │   │   └── Home.css
│   │   ├── About/
│   │   │   ├── About.jsx
│   │   │   └── About.css
│   │   ├── Services/
│   │   │   ├── Services.jsx
│   │   │   └── Services.css
│   │   ├── Blog/
│   │   │   ├── Blog.jsx
│   │   │   └── Blog.css
│   │   ├── Marques/         
│   │   │   ├── Marques.jsx
│   │   │   └── Marques.css
│   │   ├── MarqueDetails/    
│   │   │   ├── MarqueDetails.jsx
│   │   │   └── MarqueDetails.css
│   │   └── Contact/
│   │       ├── Contact.jsx
│   │       └── Contact.css
│   ├── data/                
│   │   ├── MostReplayed.js    
│   ├── sections/             
│   ├── App.jsx               # Main app component
│   ├── App.css               # Global styles
│   ├── index.js              # Entry point
├── package.json
├── package-lock.json
└── README.md
```

### 📄 Pages Overview

1. HOME 🏠

- Landing page with hero section
- Featured car brands
- Popular rental cars
- Special offers and promotions
- Call-to-action buttons

2. ABOUT US ℹ️

- Company history and mission
- Team information
- Core values
- Why choose us section
- Customer testimonials

3. SERVICES 💼

- Rental packages (daily, weekly, monthly)
- Additional services (insurance, GPS, driver)
- Pricing information
- Booking process explanation
- Terms and conditions

4. BLOG 📝

- Automotive articles and news
- Car maintenance tips
- Travel guides
- Industry updates
- Categorized posts

5. MARQUES 🚘

- Grid/List of all available car brands
- Brand logos and descriptions
- Quick stats (models available, starting price)
- Click to view brand-specific models
- Filter and search functionality

#### Marque Details Sub-page
When a brand is selected, users are navigated to a dedicated page showing:

- All available models for that brand
- Car specifications (seats, transmission, fuel type)
- Pricing per day
- High-quality car images
- Booking button for each model

6. CONTACT 📞

- Contact form (name, email, phone, message)

### 🎮 Usage

#### Navigation

- Use the navbar to navigate between different sections
- Click on any car brand in the Marques page to view its models
- Browse through blog posts and click to read full articles
- Fill out the contact form to send inquiries

#### Browsing Cars

1 - Go to Marques page
2 - Select your preferred car brand
3 - Browse through available models
4 - View specifications and pricing
5 - Click "Book Now" for your chosen vehicle

### 🛠️ Technologies Used

#### Core Technologies

- React.js (v18.x) - UI library
- React Router DOM - Client-side routing
- JavaScript (ES6+) - Programming language
- CSS3 - Styling
- HTML5 - Markup

#### Development Tools

- Create React App - Project bootstrapping
- npm/yarn - Package management
- Git - Version control
- VS Code - Code editor

#### Key React Concepts Applied

- Functional Components
- React Hooks (useState, useEffect, useParams)
- Component Props
- Conditional Rendering
- List Rendering with map()
- Event Handling
- React Router Navigation

### 🛣️ Routing System

```
import { BrowserRouter, Routes, Route } from 'react-router-dom';

<BrowserRouter>
  <Routes>
    <Route path="/" element={<Home />} />
    <Route path="/about" element={<About />} />
    <Route path="/services" element={<Services />} />
    <Route path="/blog" element={<Blog />} />
    <Route path="/marques" element={<Marques />} />
    <Route path="/marques/:brandId" element={<MarqueDetails />} />
    <Route path="/contact" element={<Contact />} />
  </Routes>
</BrowserRouter>
```

#### Dynamic Routing
The marques page uses dynamic routing:

- /marques - Shows all brands
- /marques/mercedes - Shows Mercedes models
- /marques/bmw - Shows BMW models
- /marques/audi - Shows Audi models

### 👥 Authors

#### Houssam Mnasfa - Initial work - MNASFA

