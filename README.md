# NOVA FORM - Luxury Men's Footwear & Admin Dashboard

A comprehensive, responsive men's footwear e-commerce website with a dedicated administration dashboard tailored for the Pakistani market. Inspired by modern editorial footwear brands with an original aesthetic identity.

---

## 1. Technologies Used
- **Core Markup:** Semantic HTML5
- **Styling:** Custom CSS3 (`front-site/assets/css/style.css`, `dashboard/assets/css/dashboard.css`) & CSS Variables
- **Grid & Framework:** Bootstrap 5.3.3 (loaded via CDN)
- **Icons:** Bootstrap Icons 1.11.3
- **Typography:** Google Fonts (`Plus Jakarta Sans` & `Playfair Display`)
- **Interactions:** Minimal vanilla JavaScript for essential UI actions (image gallery switcher, cart counter & line calculations, size/color selectors, offcanvas menus, modals)
- **No Heavy Frameworks:** Pure static files without React, Vue, Angular, Tailwind, Webpack, Node runtime dependencies, databases, or payment gateways.

---

## 2. Project Architecture & Structure

```text
stepupstore/
├── front-site/
│   ├── index.php                # Luxury homepage (Hero, Categories, Best Sellers, Promo, New Arrivals, Reviews)
│   ├── shop.php                 # Product catalog with search, filters (size, price, category), sorting & pagination
│   ├── category.php             # Category showcase (Formal Shoes & Loafers)
│   ├── product-details.php      # Product detail with thumbnail gallery, EU 39-46 sizes, specs tabs, related items
│   ├── cart.php                 # Shopping bag with quantity adjustments, free shipping calculation, and item removal
│   ├── checkout.php             # 2-column checkout with Pakistani address fields, COD & bank transfer, confirmation modal
│   ├── login.php                # Customer sign in
│   ├── register.php             # Customer registration
│   ├── forgot-password.php      # Password recovery demo
│   ├── account.php              # Customer profile & recent order overview
│   ├── orders.php               # Customer order history table
│   ├── order-details.php        # Order status timeline, items, and delivery address
│   ├── wishlist.php             # Saved footwear items with quick add to bag
│   ├── about.php                # Brand story, Goodyear-welted craftsmanship, Pakistani leather heritage
│   ├── contact.php              # Contact form & store ateliers in Lahore, Karachi, and Islamabad
│   ├── size-guide.php           # EU 39–46 size chart with centimeters and foot measuring guide
│   ├── assets/
│   │   ├── css/
│   │   │   ├── style.css        # Frontend master styles & design tokens
│   │   │   └── responsive.css   # Mobile and tablet breakpoints
│   │   └── js/
│   │       └── main.js          # Cart count, gallery switcher, variant selector, calculations
│   └── README.md
│
├── dashboard/
│   ├── index.php                # Executive overview with KPI cards, CSS velocity chart, recent orders, low stock
│   ├── login.php                # Admin portal login
│   ├── register.php             # Staff registration
│   ├── forgot-password.php      # Password recovery
│   ├── products.php             # 24-product catalog with search, category filters, and delete modal
│   ├── product-add.php          # Add footwear model with EU 39-46 variant matrix, image preview, pricing
│   ├── product-edit.php         # Prepopulated product editing form
│   ├── categories.php           # Category hierarchy table & Add Category modal
│   ├── brands.php               # Atelier labels (Black Label, Artisan, Heritage, Urban)
│   ├── inventory.php            # Real-time stock levels with Low Stock badges & stock adjustment modal
│   ├── orders.php               # Nationwide order list with status and payment filters
│   ├── order-details.php        # Order management, tracking updates, and staff notes
│   ├── customers.php            # Client directory with lifetime spend in PKR
│   ├── customer-details.php     # Customer profile and purchase history
│   ├── reviews.php              # Customer review moderation (Approve, Hide, Delete)
│   ├── banners.php              # Store campaign banner manager
│   ├── website-content.php      # Homepage hero, promo, and footer CMS text editor
│   ├── settings.php             # Delivery fees (PKR 250), free delivery threshold (PKR 10,000), policies
│   ├── profile.php              # Admin profile and credentials form
│   ├── assets/
│   │   ├── css/
│   │   │   ├── dashboard.css    # Admin master styles & dark slate sidebar
│   │   │   └── responsive.css   # Responsive collapse and mobile offcanvas
│   │   └── js/
│   │       └── dashboard.js     # Sidebar toggle, image upload preview, delete/stock modals
│   └── README.md
│
└── README.md
```

---

## 3. How to Run Locally

### Option A: VS Code Live Server (Recommended)
1. Open the project folder in **Visual Studio Code**.
2. Right-click on `front-site/index.php` and choose **"Open with Live Server"**.
3. To view the admin console, open `dashboard/index.php` with Live Server.

### Option B: Local Web Server (Laragon / XAMPP / Python)
- Access via your browser at `http://localhost/stepupstore/front-site/` or `http://localhost/stepupstore/dashboard/`.
- Alternatively, run Python's built-in server from the root directory:
  ```bash
  python -m http.server 8000
  ```
  Then visit `http://localhost:8000/front-site/`.

---

## 4. Pakistani Footwear Details & Currency
- **Currency:** All prices are formatted in **PKR** (Pakistani Rupee), e.g., PKR 4,499 to PKR 16,999.
- **Delivery:** Nationwide complimentary delivery on orders above PKR 10,000 (otherwise PKR 250).
- **Payment:** Cash on Delivery (COD), Direct Bank Transfer (Meezan / HBL / Alfalah), and demo card payment.
- **Shoe Sizes:** Standard European sizing **EU 39 through 46** with centimeter length conversions in `size-guide.php`.
- **Traditional Footwear:** Authentic Pakistani styles included (Khyber Peshawari Chappal, Kaptaan Chappal, and Balochi sandals).
