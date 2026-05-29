# Grace & Glamour — Ultra Luxury Salon Website v4.0

> Surat's Premier Luxury Beauty & Bridal Salon Platform  
> Fully responsive · Admin + Team system · Production-ready · Vercel-deployable

---

## 🌟 What's Inside

| Feature | Details |
|---|---|
| **Brand Loader** | Animated gem + luxury typography + progress bar |
| **Custom Cursor** | Dual-ring magnetic cursor (desktop only) |
| **Hero Section** | Cinematic dark luxury, floating stat cards, gold gradients |
| **Services** | Full searchable catalog — 40+ services across 12 categories |
| **Trending** | Horizontal scroll rail with hot-badge services |
| **Coupons** | 6 active codes with tap-to-copy |
| **Branches** | 3 Surat branches — Vesu, Rander, Jahangirpura |
| **Gallery** | Auto-scrolling infinite marquee |
| **Reviews** | 6 verified Google/Justdial review cards |
| **Booking** | Full calendar + time slots + stylist selection |
| **Admin Panel** | Dashboard, bookings, revenue charts, services, team, attendance, customers, coupons |
| **Team Panel** | Billing, attendance tracker, calendar, appointments |
| **WhatsApp FAB** | Official WA icon with pulse animation |

---

## 🚀 Deploy to Vercel (Free)

### Option 1 — Vercel CLI
```bash
npm install -g vercel
vercel login
vercel --prod
```

### Option 2 — GitHub + Vercel Dashboard
1. Push this folder to a GitHub repo
2. Go to [vercel.com](https://vercel.com) → Import Project
3. Select your repo → Deploy
4. ✅ Live in under 60 seconds

---

## 📁 File Structure

```
grace-glamour/
├── index.html        ← Complete single-file application
├── vercel.json       ← Vercel deployment config
└── README.md         ← This file
```

---

## 🔐 Demo Login Credentials

### Admin
| Field | Value |
|---|---|
| Email | admin@gracenglamour.com |
| Password | Admin@GG2025 |

### Team Members
| ID | Name | MPIN |
|---|---|---|
| GG-001 | Priya Sharma | 1234 |
| GG-002 | Anjali Patel | 2345 |
| GG-003 | Kavya Mehta | 3456 |
| GG-004 | Riya Joshi | 4567 |

---

## 🔧 Customisation Guide

### Update WhatsApp Number
Search for `9876543210` in `index.html` → replace with your number.

### Update Branch Info
Search for `Vesu Branch`, `Rander Branch`, `Jahangirpura Branch` in HTML — update addresses.

### Update Google Rating / Reviews
Search for `DB.reviews` in the script — add/edit review objects.

### Update Services / Prices
Find `DB.svcs` in the script — each service object:
```js
{
  id: 'unique-id',
  cat: 'category-id',   // must match a DB.cats id
  name: 'Service Name',
  desc: 'Description',
  price: 500,           // starting price in ₹
  maxPrice: 2000,       // optional: shows price range
  dur: '45 min',
  hot: true             // shows 🔥 Trending badge
}
```

### Add Google Sheets Database (Free)
1. Create a Google Sheet with columns: Name, Phone, Service, Date, Time, Branch, Stylist
2. Tools → Apps Script → paste the API handler script
3. Deploy as Web App (anyone can access)
4. Replace `confirmBooking()` fetch call with your Apps Script URL

---

## 📱 Browser Support

- Chrome 90+ ✅
- Safari 14+ ✅
- Firefox 88+ ✅
- Edge 90+ ✅
- Android Chrome ✅
- iOS Safari ✅

---

## 📞 Contact & Support

**Grace & Glamour Luxury Salon**  
- 🌐 gracenglamour.site  
- 📸 @grace_n_glamour  
- 📍 Vesu · Rander · Jahangirpura, Surat  

---

*Built with ♥ in Surat, India · v4.0 Final*
