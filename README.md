#  Waste Management & Recycling Platform

![License](https://img.shields.io/badge/license-MIT-green) ![React](https://img.shields.io/badge/React-18.3.1-blue) ![Firebase](https://img.shields.io/badge/Firebase-10.13.0-yellow) ![TailwindCSS](https://img.shields.io/badge/Tailwind_CSS-3.4.10-teal) 

A full-stack React & Firebase web application connecting users, scrap dealers, NGOs, and government bodies to streamline waste recycling, scrap selling, creative reuse, and community engagement.

---

## Table of Contents  
- [Project Overview](#project-overview)  
- [Tech Stack & Dependencies](#tech-stack--dependencies)  
- [Project Workflow](#project-workflow)  
- [Features](#features)  
- [Installation & Setup](#installation--setup)  
- [Usage](#usage)  
- [User Roles & Route Protection](#user-roles--route-protection)  
- [Project Structure](#project-structure)  
- [Contributing](#contributing)  
- [License](#license)  

---

## Project Overview

EcoCreate empowers communities to efficiently manage waste by connecting diverse stakeholders. Users can list scrap products for sale, bid on scrap, submit creative projects transforming waste, and access governmental waste management schemes. Real-time updates ensure responsiveness using Firebase services.

---

## Tech Stack & Dependencies

- **React** v18.3.1  
- **Firebase** v10.13.0 (Firestore, Auth, Storage)  
- **React Router DOM** v6.26.1  
- **Tailwind CSS** v3.4.10 (Styling)  
- **Lottie React** v2.4.0 (Animations)  
- **React Hot Toast** v2.4.1 (Notifications)  
- **React i18next/i18next** (Intl support)  
- **Axios** (HTTP requests)  
- **React Icons** (Icons)  
- **Testing:** React Testing Library  
- Other tooling: Web Vitals, React Redux (partial usage)  

_All dependencies and versions are based on package.json._

---

## Project Workflow

1. **User Registration & Authentication:**  
   - Users select roles (user, scrap dealer, NGO) and optionally provide geolocation data.  
2. **Landing & Role-Based Views:**  
   - Customized home pages and dashboards per role with access restrictions.  
3. **Scrap Product Management:**  
   - Scrap dealers add/edit scrap listings with images and location info.
4. **Product Browsing and Filtering:**  
   - Users browse and filter scrap by category, price, state, city, and distance (calculated by Haversine formula).  
5. **Bidding and Negotiation:**  
   - Scrap dealers bid on items; users can comment and finalize deals.  
6. **Creative Idea Submission:**  
   - Users share innovative projects categorized by cooking, arts & crafts, and school projects.  
7. **Government Schemes & Messaging:**  
   - NGOs and users view government scheme updates and communicate community issues via CleanConnect.  
8. **Real-time Updates:**  
   - Firestore listeners update bids, comments, and product info instantly.  
9. **Route Protection:**  
   - Role-based route guards restrict unauthorized access.  
10. **UI/UX Enhancements:**  
    - Responsive design with Tailwind CSS and engaging Lottie animations. 

---

## Features

- User signup/login and role-based access (user, scrap dealer, NGO)  
- Add, update, and delete scrap products with images  
- Browse and filter scrap products by multiple criteria including geolocation proximity  
- Bidding mechanism with real-time feedback  
- Commenting system to track negotiation and deal status  
- Submit and browse creative ideas/projects  
- Government schemes notifications and updates  
- Personalized dashboards by role  
- Responsive design with compelling animations  
- Scroll-to-top on navigation for smooth UX  

---

## Installation & Setup

### Prerequisites

- Node.js v14 or higher  
- Firebase account with Firestore, Authentication, and Storage enabled

### Setup Steps

1. **Clone repository:**

   - git clone https://github.com/amansingh4012/Resort-It-
   - cd Resort-it
   - npm install


2. **Firebase Configuration:**
   - Go to [Firebase Console](https://console.firebase.google.com/)
   - Create new project
   - Enable Authentication (Email/Password)
   - Create Firestore database
   - Copy your Firebase config to `src/firebase/Firebase.jsx`

3. **Start development server:**

   - npm start
   - Open your browser at `http://localhost:3000`

---

## Usage

- Register and login as your chosen role.  
- Users can list scrap, submit ideas, place bids, and track deals.  
- Scrap dealers manage listings and bid on products.  
- NGOs can post governmental updates and engage via messaging features.  
- Use filters on category pages to find scrap by location and pricing.  
- Place bids and comments to facilitate transactions immediately.  

---

## User Roles & Route Protection

| Role        | Access Permissions                         |
|-------------|--------------------------------------------|
| User        | Submit/view scrap, place bids, submit ideas, comment on deals, user dashboard |
| Scrap Dealer| Add scrap products, bid on listings, manage deals, scrap dealer dashboard |
| NGO         | Post government schemes, receive messages, access NGO features |
| Owner       | Manage all product listings, full dashboard access |

Protected routes ensure users can only access pages authorized for their roles, enhancing security.

---

## Project Structure
src/ <br>
├── assets/ # Images & icons <br>
├── components/ # Reusable UI components & pages <br>
├── context/ # Global state management (Context API) <br>
├── css/ # Styling and animations <br>
├── firebase/ # Firebase config and initialization <br>
├── pages/ # Main app pages per feature <br>
├── protectedRoute/ # Role-based routing guards<br>
├── App.js # Main router and app bootstrap<br>
├── index.js # Entry point<br>



---

## Contributing

Contributions are welcome! To contribute:  
1. Fork the repository  
2. Create a feature branch (`git checkout -b feature/your-feature`)  
3. Commit your changes (`git commit -m "Add your feature"`)  
4. Push to your fork (`git push origin feature/your-feature`)  
5. Open a Pull Request  

---

## License

This project is licensed under the MIT License.

---




