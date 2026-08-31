# PRD — Website #5: MOTION CAR

**Premium Car Wash & Auto Care Website**
**Architecture:** Astro + Cloudflare Pages
**Deployment:** Static-first, lightweight, mobile-first, local SEO focused

---

# 1. Product Overview

### Brand

**MOTION CAR**

### Industry

Car Wash / Auto Care / Vehicle Detailing

### Website Type

Local Service Business Website

Website berfungsi sebagai:
* service showcase
* price showcase
* booking/WhatsApp lead generator
* outlet information
* trust-building platform
* local SEO asset

### Primary Goal

Mengubah pengunjung menjadi pelanggan:

> **Lihat Service → Pilih Paket → Booking**

Primary conversion:

**Book via WhatsApp**

Secondary:
* Lihat Harga
* Lihat Paket
* Cari Lokasi
* Call
* Get Directions

---

# 2. Product Positioning

MOTION CAR diposisikan sebagai layanan cuci dan perawatan mobil modern dengan pengalaman yang cepat, profesional, bersih, dan terpercaya.

### Brand Promise

> **CLEAN. SHINE. MOVE.**

### Main Message

> Mobil bersih, tampil lebih baik, siap melaju.

### Supporting Message

> Perawatan kendaraan yang praktis dengan hasil bersih dan maksimal.

### Brand Personality

* energetic
* professional
* automotive
* premium
* precise
* reliable

---

# 3. Target Audience

## Primary

### Daily Car Owners

Pemilik mobil yang membutuhkan:
* cuci rutin
* cuci cepat
* perawatan kendaraan

## Secondary

### Car Enthusiasts

Membutuhkan:
* detailing
* interior cleaning
* polishing
* coating

## Tertiary

### Families / Professionals

Membutuhkan service yang:
* cepat
* mudah
* terpercaya
* dekat

---

# 4. Business Objectives

1. Meningkatkan jumlah booking.
2. Menampilkan layanan secara jelas.
3. Meningkatkan average transaction melalui package upsell.
4. Membangun trust.
5. Meningkatkan local search visibility.
6. Mempermudah pelanggan menemukan outlet.

---

# 5. Conversion Strategy

Primary:

> **Book Now**

Secondary:

> **View Services**

Tertiary:

> **Find Location**

CTA harus muncul berulang pada titik yang relevan.

---

# 6. Architecture Decision

Gunakan:

**Astro Static + Cloudflare Pages**

Tidak menggunakan database untuk MVP.

Static data:

```text
src/data/
├── services.ts
├── packages.ts
├── locations.ts
├── faqs.ts
└── testimonials.ts
```

Booking langsung menuju WhatsApp.

Tidak membuat booking engine pada MVP.

---

# 7. Sitemap

```text
/
├── /services
├── /packages
├── /locations
├── /about
├── /faq
├── /contact
└── /privacy
```

P0:

```text
/
├── /services
├── /packages
└── /contact
```

P1:

```text
/locations
/about
/faq
```

---

# 8. Homepage Funnel

```text
Hero
↓
Trust Indicators
↓
Popular Services
↓
Pricing / Packages
↓
Why Motion Car
↓
Before / After
↓
Process
↓
Location
↓
Testimonials
↓
FAQ
↓
Final Booking CTA
↓
Footer
```

---

# 9. Announcement Bar

Contoh:

> **WEEKDAY SPECIAL — CAR WASH FROM Rp XX.XXX**

CTA:

**See Packages**

Promo harus configurable dan dapat dinonaktifkan.

---

# 10. Navbar

Desktop:

```text
MOTION CAR

Services
Packages
Locations
About
FAQ

                    Book Now
```

Mobile:

```text
MOTION
CAR                 ☰
```

Primary CTA:

**Book Now**

---

# 11. Hero Section

### Headline

> **MAKE YOUR CAR
> LOOK ITS BEST.**

### Supporting Copy

> Professional car wash and detailing services designed to keep your vehicle clean, fresh, and ready to move.

CTA:

**Book Now**

Secondary:

**View Services**

---

# 12. Hero Visual

Visual utama:
* glossy clean car
* water droplets
* foam
* detailing process
* dark automotive environment

Style:

high contrast, cinematic, premium.

Desktop:

```text
┌───────────────────────────┬─────────────────────┐
│ MAKE YOUR CAR             │                     │
│ LOOK ITS BEST             │    HERO CAR IMAGE   │
│                           │                     │
│ [Book Now]                │                     │
│ [Services]                │                     │
└───────────────────────────┴─────────────────────┘
```

---

# 13. Trust Indicators

Immediately setelah hero:

```text
✓ Professional Team
✓ Quality Products
✓ Fast Service
✓ Easy Booking
```

Jika tersedia, dapat ditambahkan:

```text
10K+ Cars Served
4.8★ Customer Rating
```

Hanya gunakan angka jika benar-benar tersedia.

---

# 14. Service Section

Headline:

> **CAR CARE, YOUR WAY**

Services:

### Basic Car Wash

Cuci eksterior untuk perawatan rutin.

### Wash & Vacuum

Eksterior + interior vacuum.

### Interior Cleaning

Membersihkan interior kendaraan secara menyeluruh.

### Car Detailing

Perawatan detail untuk tampilan kendaraan.

### Polish

Mengembalikan kilau dan membantu memperbaiki tampilan permukaan.

### Wax / Protection

Perlindungan dan finishing tambahan.

---

# 15. Service Card

```text
[IMAGE]

BASIC CAR WASH

Clean exterior.
Quick and simple.

From
Rp XX.XXX

[Book Service]
```

CTA:

**Book Service**

---

# 16. Package Section

Headline:

> **CHOOSE YOUR LEVEL OF CLEAN**

Packages:

### QUICK CLEAN

```text
Exterior Wash
Dry
Tire Cleaning
```

### COMPLETE CLEAN

```text
Exterior Wash
Interior Vacuum
Dashboard Cleaning
Tire Cleaning
```

### DETAIL PACKAGE

```text
Deep Cleaning
Interior Detail
Exterior Detail
Finishing
```

Pricing:

```text
Rp XX.XXX
Rp XX.XXX
Rp XXX.XXX
```

---

# 17. Package Comparison

Desktop:

| Feature           | Quick Clean | Complete Clean | Detail |
| ----------------- | ----------: | -------------: | -----: |
| Exterior Wash     |           ✓ |              ✓ |      ✓ |
| Drying            |           ✓ |              ✓ |      ✓ |
| Vacuum            |           — |              ✓ |      ✓ |
| Interior Cleaning |           — |              ✓ |      ✓ |
| Detailing         |           — |              — |      ✓ |
| Finishing         |           — |              — |      ✓ |

Mobile berubah menjadi stacked cards.

---

# 18. Recommended Package

Satu package dapat diberi label:

> **MOST POPULAR**

Tujuannya meningkatkan conversion dan average order value.

Jangan membuat package terlalu banyak.

Ideal MVP:

**3–4 packages.**

---

# 19. Why Motion Car

Headline:

> **MORE THAN JUST A CAR WASH**

Benefits:

### Professional Process

Tim mengikuti proses service yang terstruktur.

### Quality Products

Gunakan produk perawatan kendaraan yang sesuai.

### Attention to Detail

Area kecil yang sering terlewat tetap diperhatikan.

### Convenient

Booking mudah dan proses praktis.

---

# 20. Before / After

Section visual conversion.

Headline:

> **SEE THE DIFFERENCE**

Layout:

```text
BEFORE            AFTER

[ IMAGE ]         [ IMAGE ]
```

Jika menggunakan slider, gunakan implementasi lightweight.

Alternatif MVP:

dua image berdampingan.

Jangan memakai library comparison berat.

---

# 21. Service Process

Headline:

> **HOW IT WORKS**

### 01 — Book

Pilih service dan hubungi Motion Car.

### 02 — Bring Your Car

Datang ke outlet pada waktu yang disepakati.

### 03 — We Clean

Tim melakukan service sesuai package.

### 04 — Drive Away

Mobil bersih dan siap digunakan.

---

# 22. Automotive Detail Section

Headline:

> **DETAILS MATTER**

Copy:

> From wheels to dashboard, every part of your car deserves proper care.

Visual:
* wheel cleaning
* dashboard
* seats
* exterior detailing
* microfiber process

Tujuan:

Meningkatkan perceived quality.

---

# 23. Location Section

Headline:

> **FIND YOUR MOTION CAR**

Location card:

```text
MOTION CAR Pekanbaru

Jl. Example No. 123
Pekanbaru, Riau

Open Today
08:00 – 21:00

[Get Directions]
[Book Now]
```

---

# 24. Location Data

Jika multi-outlet:

```text
Pekanbaru
Dumai
Padang
Medan
```

Actual cities harus mengikuti area bisnis.

---

# 25. Testimonials

Headline:

> **DRIVERS LOVE THE DIFFERENCE**

3 testimonial cards.

Contoh:

```text
★★★★★

"Mobil jadi jauh lebih bersih.
Prosesnya juga cepat."

— Customer
```

Gunakan testimonial asli pada production.

---

# 26. FAQ

Headline:

> **CAR WASH FAQ**

Questions:

### Berapa lama proses cuci mobil?

Tampilkan estimasi berdasarkan service aktual.

### Apakah harus booking?

Jelaskan kebijakan outlet.

### Apakah menerima semua jenis mobil?

Jelaskan kategori kendaraan yang diterima.

### Apakah tersedia detailing?

Ya, jika layanan tersedia.

### Apakah bisa booking melalui WhatsApp?

Ya.

### Apakah ada harga berbeda untuk SUV?

Jika memang ada, jelaskan.

### Apakah bisa datang langsung?

Jelaskan walk-in policy.

---

# 27. Final CTA

Headline:

> **READY TO MAKE IT SHINE?**

Copy:

> Book your next car wash and give your vehicle the care it deserves.

CTA:

**Book Now**

Secondary:

**View Packages**

---

# 28. Contact

Informasi:

```text
WhatsApp
Phone
Address
Opening Hours
```

CTA:

**Chat on WhatsApp**

---

# 29. Footer

```text
MOTION CAR

Clean. Shine. Move.

SERVICES
Car Wash
Interior Cleaning
Detailing
Polish
Protection

PACKAGES
Quick Clean
Complete Clean
Detail

COMPANY
About
Locations
FAQ
Contact

FOLLOW
Instagram
TikTok
Facebook

CONTACT
WhatsApp
Phone
Email

© 2026 MOTION CAR

Privacy Policy
Terms
```

---

# 30. Visual Design Direction

MOTION CAR harus terasa seperti **premium automotive care brand**.

### Style

* dark
* bold
* technical
* energetic
* premium
* clean

Visual:
* glossy cars
* water
* foam
* metal
* black surfaces
* high contrast photography

Avoid:
* generic blue car wash template
* cartoon car graphics
* excessive gradients
* neon overload
* excessive animation

---

# 31. Color System

Recommended:

```text
Carbon Black
#0B0D0E

Graphite
#171A1D

Electric Red
#E21B2D

Light Gray
#E9ECEF

Off White
#F5F5F3

White
#FFFFFF
```

Primary:

**Carbon Black**

Accent:

**Electric Red**

Background:

**Graphite / Off White**

---

# 32. Typography

### Display

**Barlow Condensed / Archivo Black**

Automotive, bold, technical.

### Body

**Inter**

Hero:

```text
64–88px desktop
42–52px mobile
```

Section:

```text
42–54px desktop
30–38px mobile
```

---

# 33. UI Components

```text
AnnouncementBar
Navbar
MobileMenu
Button
Hero
TrustBadge
ServiceCard
PackageCard
PackageComparison
BeforeAfter
ProcessSteps
BenefitCard
LocationCard
TestimonialCard
FAQ
ContactCTA
Footer
```

---

# 34. Repository Structure

```text
motion-car-website/

├── public/
│   ├── images/
│   ├── icons/
│   └── favicon.svg
│
├── src/
│   ├── components/
│   │   ├── ui/
│   │   ├── navigation/
│   │   ├── services/
│   │   ├── packages/
│   │   ├── locations/
│   │   └── sections/
│   │
│   ├── layouts/
│   │   └── BaseLayout.astro
│   │
│   ├── pages/
│   │   ├── index.astro
│   │   ├── services.astro
│   │   ├── packages.astro
│   │   ├── locations.astro
│   │   ├── about.astro
│   │   ├── faq.astro
│   │   └── contact.astro
│   │
│   ├── data/
│   │   ├── services.ts
│   │   ├── packages.ts
│   │   ├── locations.ts
│   │   ├── faqs.ts
│   │   └── testimonials.ts
│   │
│   ├── seo/
│   │   └── schema.ts
│   │
│   └── styles/
│       └── global.css
│
├── astro.config.mjs
├── package.json
├── tsconfig.json
├── wrangler.toml
├── README.md
└── .env.example
```

---

# 35. Service Data Model

```typescript
{
  id: string,
  slug: string,
  name: string,
  description: string,
  price?: number,
  duration?: string,
  image?: string,
  features: string[],
  featured: boolean,
  available: boolean
}
```

---

# 36. Package Data Model

```typescript
{
  id: string,
  slug: string,
  name: string,
  description: string,
  price: number,
  features: string[],
  popular?: boolean,
  image?: string,
  available: boolean
}
```

---

# 37. Booking Flow

MVP:

```text
Homepage
   ↓
Book Now
   ↓
WhatsApp
   ↓
Customer selects service
   ↓
Motion Car confirms
```

Pre-filled message:

> Halo Motion Car, saya ingin booking [Service/Package]. Mohon informasi jadwal yang tersedia.

Jika customer berasal dari halaman package tertentu, nama package otomatis dimasukkan.

---

# 38. Local SEO

Keyword cluster:

```text
cuci mobil [city]
cuci mobil terdekat
car wash [city]
car wash near me
cuci mobil murah [city]
detailing mobil [city]
salon mobil [city]
polish mobil [city]
interior mobil [city]
```

Jika ada outlet:

```text
cuci mobil [district]
car wash [district]
```

---

# 39. SEO Metadata

Homepage:

> MOTION CAR — Car Wash & Auto Care | [City]

Description:

> Car wash, interior cleaning, detailing, polish, dan auto care di [City]. Lihat layanan dan booking Motion Car melalui WhatsApp.

Services:

> Car Wash & Auto Care Services | MOTION CAR

Locations:

> MOTION CAR [City] — Location, Hours & Services

---

# 40. Structured Data

Implement:

```text
Organization
LocalBusiness
Automotive-related Service data
BreadcrumbList
```

Untuk outlet:
* name
* address
* phone
* opening hours
* geo
* URL

Gunakan data aktual.

---

# 41. Technical SEO

Wajib:
* sitemap
* robots
* canonical
* Open Graph
* metadata
* semantic HTML
* image alt
* descriptive URLs
* internal links
* structured data

---

# 42. Image Strategy

Automotive photography memiliki file besar.

Rules:
* AVIF/WebP
* responsive images
* explicit dimensions
* lazy load below fold
* preload/prioritize hero image
* compressed before upload

Before/after image harus memiliki ukuran optimal.

---

# 43. Performance

Target:

```text
Performance      90+
Accessibility    95+
Best Practices   95+
SEO              95+
```

Core Web Vitals:

```text
LCP < 2.5s
INP < 200ms
CLS < 0.1
```

---

# 44. JavaScript Policy

Default:

**Zero JS.**

JS hanya untuk:
* mobile menu
* package filtering jika dibutuhkan
* optional before/after interaction

FAQ menggunakan native `<details>`.

Tidak menggunakan:
* React untuk seluruh website
* GSAP
* heavy carousel
* heavy comparison slider
* animation framework

---

# 45. Analytics

Gunakan:

**Cloudflare Web Analytics**

Track:

```text
Book Now Click
WhatsApp Click
Service View
Package View
Location Click
Get Directions
Phone Click
```

---

# 46. Accessibility

Wajib:
* semantic HTML
* keyboard navigation
* focus state
* proper labels
* accessible FAQ
* sufficient contrast
* alt text
* accessible mobile menu
* touch-friendly CTA
* reduced motion

---

# 47. Security

MVP tidak menyimpan customer data.

Rules:
* HTTPS
* no frontend secrets
* no exposed API keys
* external URL validation
* dependency audit
* minimal third-party scripts

---

# 48. Cloudflare Architecture

```text
Customer
   ↓
Cloudflare CDN
   ↓
Cloudflare Pages
   ↓
Astro Static
```

Tidak perlu:
* D1
* R2
* Durable Objects
* Workers API

untuk MVP.

---

# 49. Bundle Requirement

Target:

> **Compressed Worker bundle jauh di bawah 3 MiB.**

Rules:
* static generation
* minimal JS
* minimal dependencies
* no heavy UI library
* no heavy server dependencies
* image optimization
* bundle analysis

Production build wajib menggunakan webpack dan diverifikasi sebelum deployment.

---

# 50. Multilingual

Support:

**Bahasa Indonesia + English**

Recommended:

```text
/id/
/en/
```

Default:

**Indonesia**

Translation:

```text
src/data/i18n/
├── id.ts
└── en.ts
```

---

# 51. Out of Scope

Tidak membangun:
* customer login
* online payment
* booking database
* appointment dashboard
* employee dashboard
* vehicle tracking
* loyalty program
* CRM
* custom CMS
* D1
* complex scheduling system
* live queue
* mobile application

---

# 52. Future Expansion

Jika booking volume tinggi:

```text
booking slots
appointment confirmation
customer profiles
service history
loyalty
automated reminders
staff management
```

Tidak termasuk MVP.

---

# 53. Definition of Done

### Brand

* [ ] Premium automotive aesthetic
* [ ] Strong Motion Car identity
* [ ] High-quality car photography
* [ ] Dark/high-contrast design
* [ ] Responsive mobile-first

### Services

* [ ] Service listing
* [ ] Package listing
* [ ] Package comparison
* [ ] Pricing
* [ ] Service details

### Conversion

* [ ] Book Now
* [ ] WhatsApp booking
* [ ] Service CTA
* [ ] Package CTA
* [ ] Location CTA
* [ ] Phone CTA

### Trust

* [ ] Benefits
* [ ] Process
* [ ] Before/after
* [ ] Testimonials
* [ ] FAQ

### SEO

* [ ] Metadata
* [ ] Sitemap
* [ ] Robots
* [ ] Custom canonical configuration
* [ ] Open Graph
* [ ] Local SEO
* [ ] Structured data

### Performance

* [ ] Static Astro
* [ ] Optimized images
* [ ] Minimal JS
* [ ] Minimal dependencies
* [ ] Lighthouse 90+
* [ ] Core Web Vitals optimized

### Cloudflare

* [ ] Cloudflare Pages
* [ ] Astro Cloudflare configuration
* [ ] Webpack production build verified
* [ ] Bundle analyzed
* [ ] Under 3 MiB compressed target
* [ ] Environment variables documented
* [ ] Deployment tested

---

# 54. Implementation Priority

## Phase 1 — Foundation

```text
Astro
Cloudflare
Global CSS
Typography
Colors
Base Layout
SEO
```

## Phase 2 — Services

```text
Services
Packages
Pricing
Comparison
```

## Phase 3 — Conversion

```text
Book Now
WhatsApp
Contact
Location
```

## Phase 4 — Trust

```text
Why Motion Car
Process
Before/After
Testimonials
FAQ
```

## Phase 5 — SEO

```text
Local SEO
Schema
Metadata
Location pages
Internal links
```

## Phase 6 — Optimization

```text
Image optimization
Accessibility
Performance
Bundle analysis
Cloudflare QA
```

---

# 55. Final Product Direction

MOTION CAR harus terasa seperti **premium automotive care experience**, bukan sekadar website tempat cuci mobil.

Customer journey:

```text
SEE THE CAR
     ↓
SEE THE RESULT
     ↓
CHOOSE SERVICE
     ↓
CHECK PRICE
     ↓
BOOK
```

Visual principle:

> **Dark automotive aesthetic + bold typography + dramatic vehicle photography + strong red accent + clear service/package hierarchy.**

Technical principle:

> **Astro static-first + Cloudflare Pages + minimal JavaScript + centralized service/package data + WhatsApp booking + local SEO.**

**PRD Website #5 — MOTION CAR selesai.**
