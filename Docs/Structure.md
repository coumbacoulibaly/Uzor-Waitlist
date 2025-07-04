# Uzor Founders Circle – MVP Structure

## ✅ Core Goals of the MVP

- Collect email + business name from signups  
- Generate unique referral links for each user  
- Track how many people each user refers  
- Display a basic leaderboard (optional but powerful)  
- Allow admin to export/view participants and rankings  
- Be visually aligned with the Uzor brand  

---

## 🧱 Frontend Pages & Sections

| Page/Section         | Purpose                                                                 |
|----------------------|-------------------------------------------------------------------------|
| `/` (Landing Page)   | Main public page for explaining the program and collecting signups     |
| `/thanks`            | Confirmation + show referral link + # of referrals                     |
| `/leaderboard`       | (Optional) Show top referrers (name + #referrals)                      |
| `/admin` (Hidden)    | Admin-only view to export data and track user rankings                 |

---

## 🧩 Frontend Components

### Landing Page Components

- 🧭 Navigation bar (Logo + "Join" CTA)  
- 🎯 Hero section (Headline + signup form)  
- 📊 "How It Works" section (3 or 4-step visual)  
- 🎁 "What You'll Get" section (benefits grid)  
- 🔁 Referral mechanic explanation  
- 🥇 Leaderboard preview (optional)  
- 📥 Signup form: name, business name, email  
- ✅ Footer (social links, legal, etc.)

---

## 🔧 Backend / Logic (Firebase-friendly)

| Feature               | Description                                                                 |
|-----------------------|-----------------------------------------------------------------------------|
| **Database**          | Store users with name, email, business name, referrer ID, referral count    |
| **Referral Tracking** | Store referrer ID when someone signs up using a ?ref= link                |
| **Referral Links**    | Auto-generate unique referral link: uzor.app/?ref=ABC123 per user         |
| **Referral Count**    | Count how many signups each user generated                                 |
| **Leaderboard**       | Sort users by referral count                                                |
| **Admin View**        | Admin panel to view/export user and referral data (CSV or JSON)            |

---

## 🔑 Tech Stack Suggestions

- **Frontend**: React or plain HTML + JS  
- **Backend/DB**: Firebase Firestore  
- **Auth**: Firebase anonymous or email-based (optional)  
- **Link Tracking**: Firebase Functions or query param parsing  
- **Hosting**: GitHub Pages or Firebase Hosting  
- **Analytics**: Plausible or Firebase Analytics  

---

## 📦 MVP Deliverables Checklist

| Feature                             | Status |
|-------------------------------------|--------|
| Landing Page with Branding          | 🔲     |
| Signup Form (name + email + biz)    | 🔲     |
| Referral Link Generation            | 🔲     |
| Referral Count Tracking             | 🔲     |
| Thank You Page with Referral Link   | 🔲     |
| Leaderboard (Optional for v1)       | 🔲     |
| Admin Panel to View/Export Data     | 🔲     |
| Firebase Firestore Setup            | 🔲     |
| Firebase Hosting or GitHub Pages    | 🔲     |

---

## 👣 Next Step Options

### Option A: Start Designing the Page
Begin with **Hero section content + Figma layout** or **Cursor prompts**.

### Option B: Start Coding the Backend
Implement referral logic in Firebase or build a custom backend.

### Option C: Build a No-Code Version First
Use tools like [Tally.so](https://tally.so/) or [Softr](https://softr.io/) + Airtable to get a quick MVP.

--- 