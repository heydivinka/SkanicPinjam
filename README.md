# 🏫 **SkanicPinjam** - School Inventory & Borrowing System

![Screenshot](https://via.placeholder.com/1200x600/e0f2fe/10b981?text=SkanicPinjam+Dashboard)

Modern Laravel + React + Inertia.js app for school asset management.

## ✨ **Features**
| Module | Features |
|--------|----------|
| 👥 **Students** | CRUD, search, stats, dashboard |
| 👨‍🏫 **Teachers** | CRUD, profiles |
| 📦 **Inventory** | Barcode, categories, CRUD |
| 📱 **Borrowing** | Status tracking, reports |
| 📊 **Dashboard** | Charts, stats, animations |
| 📄 **Reports** | PDF/Excel export |

**Tech Stack:** Laravel 11, Inertia, React 18, Tailwind, Vite, Framer Motion, Lucide Icons

## 🚀 **Quick Setup**

### 1. Clone & Install
```bash
git clone <your-repo>
cd laravel-breeze-inertia
composer install --optimize-autoloader --no-dev
npm ci
```

### 2. Environment
```bash
cp .env.example .env
php artisan key:generate
```

**Edit `.env`:**
```
DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE=skanicpinjam
DB_USERNAME=root
DB_PASSWORD=
```

### 3. Database
```bash
php artisan migrate --seed
php artisan storage:link
npm run build
```

### 4. Run
```bash
php artisan serve
npm run dev
```

**Login:** Check seeder for admin credentials (admin@example.com)

**URL:** http://127.0.0.1:8000

## 📱 **Screenshots**
```
Login Page (Custom Illustration)
[Custom SVG Student/Teacher/Books]
Emerald Admin Dashboard
Sidebar Navigation (Collapsible)
Responsive Tables & Forms
PDF Export Preview
```

## 🌐 **Deployment (Free)**

### Railway.app (Recommended)
1. Push to GitHub
2. railway.com → New Project → Deploy from GitHub
3. Add MySQL DB, link env vars

### Render.com
```
New Web Service → GitHub Repo
Build: composer install
Start: vendor/bin/heroku-php-apache2
Add PostgreSQL
```

### Vercel (Frontend only)
```
npm run build
vercel --prod
```

## 🛠 **Development**

```bash
# Dev
npm run dev

# Production build
npm run build

# Lint
npm run lint

# Test
php artisan test
```

## 📚 **Structure**
```
app/Models/          # Eloquent Models
app/Http/Controllers # API Controllers
resources/js/Pages/  # Inertia Pages
resources/js/Components # UI Components
database/migrations/ # Schema
routes/             # API/Web routes
```

## 🎨 **Customization**
- **Colors**: `tailwind.config.js` emerald palette
- **Logo**: Sidebar.jsx `SkanicPinjam`
- **Theme**: Dark/Light support ready

## 🤝 **Contributing**
1. Fork repo
2. Create feature branch
3. `git push` & PR

## 📄 **License**
MIT - Free for commercial use.

## 👨‍💼 **Support**
Issues: GitHub Issues  
Discord: [Link]

---

**Made with ❤️ for Indonesian schools**

