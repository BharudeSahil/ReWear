# 👕 ReWear – Community Clothing Exchange

ReWear is a web-based platform designed to promote sustainable fashion by enabling users to exchange unused clothing through direct swaps or a point-based redemption system. The goal is to reduce textile waste by encouraging the reuse of wearable garments.

---

## 🌱 Overview

Fast fashion is one of the world's most polluting industries. ReWear seeks to counter this by enabling people to:

- Swap clothes directly with others in the community
- Earn and spend points to redeem clothes without cash
- Extend the lifecycle of garments and reduce landfill waste

---

## 🚀 Features

### 👤 User Authentication
- Email/password sign-up and login
- Secure session handling

### 🏠 Landing Page
- Platform introduction
- Featured items carousel
- Calls-to-action: “Start Swapping”, “Browse Items”, “List an Item”

### 📊 User Dashboard
- Profile details and points balance
- Overview of uploaded items
- List of ongoing and completed swaps

### 👗 Item Detail Page
- Full item description and image gallery
- Uploader’s profile information
- Options to:
  - **Request a Swap**
  - **Redeem using Points**
- Real-time item availability status

### ➕ Add New Item Page
- Upload item images
- Enter:
  - Title
  - Description
  - Category
  - Type
  - Size
  - Condition
  - Tags
- Submit form to list the item

### 🛠️ Admin Role
- Moderate and approve/reject submitted items
- Remove inappropriate or spam content
- Lightweight admin panel for easy oversight

---

## 🧱 Tech Stack

- **Framework**: Odoo (Python backend with OWL frontend)
- **Database**: PostgreSQL (via Odoo ORM)
- **Frontend**: OWL (Odoo Web Library), Bootstrap
- **Authentication**: Odoo user model extensions
- **Real-time Updates**: Longpolling / bus events
- **Dev Tools**: ESLint, Flake8, Git

---

## 🗃️ Database Models

- `res.users`: Extended with profile details and points balance
- `rewear.item`: Stores clothing details, images, tags, status
- `rewear.swap`: Tracks direct swap transactions
- `rewear.redeem`: Handles redemptions using points
- `rewear.config`: Stores dropdown values (categories, sizes, types)

---

## 🧪 How to Run Locally

1. **Clone the repository**
   ```bash
   git clone https://github.com/your-team/rewear.git
   cd rewear
2. **Navigate to the project directory**
   ```bash
   cd ReWear
3. **Install dependencies**
   ```bash
   npm install
4. **Set up environment variables**
  - Create a .env file in the root directory.
  - Add necessary variables (e.g., DATABASE_URL, JWT_SECRET).
5. **Start the development server**
    ```bash
    npm start

## Usage

**Users**: Sign up, browse items, list clothing for swap, or redeem items using points.

**Admins**: Log in to the admin panel to moderate listings and manage platform content.
