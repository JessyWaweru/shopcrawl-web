<div align="center">

# 🛍️ ShopCrawl · Web

### Four stores. One search. Zero open tabs.

**The React frontend for ShopCrawl: compare Amazon, Jumia, Kilimall and Shopify side by side, ranked by SmartRank™.**

[![Live Demo](https://img.shields.io/badge/🔴_Live_Demo-shopcrawl--frontend.onrender.com-e11d48?style=for-the-badge)](https://shopcrawl-frontend.onrender.com/)
[![Backend](https://img.shields.io/badge/Backend_Repo-shopcrawl--api-0f172a?style=for-the-badge&logo=github)](https://github.com/JessyWaweru/shopcrawl-api)

![React](https://img.shields.io/badge/React_18-61DAFB?logo=react&logoColor=black)
![React Router](https://img.shields.io/badge/React_Router-CA4245?logo=reactrouter&logoColor=white)
![Tailwind](https://img.shields.io/badge/Tailwind-06B6D4?logo=tailwindcss&logoColor=white)
![Font Awesome](https://img.shields.io/badge/Font_Awesome-528DD7?logo=fontawesome&logoColor=white)
![Render](https://img.shields.io/badge/Render-46E3B7?logo=render&logoColor=black)

<sub>⏳ Free-tier hosting: the first load may take ~45s while the API wakes up. Grab a coffee ☕</sub>

</div>

<p align="center">
  <img src="screenshots/demo.gif" width="800" alt="Demo: filter products by samsung, open the TV, and see four stores ranked by SmartRank">
</p>

---

## 📸 Screenshots

| 🏠 Home | 🏆 SmartRank™ |
|:---:|:---:|
| ![Home](screenshots/Shopcrawl-home-screenshot-l.png) | ![SmartRank](screenshots/shopcrawl-smartrank-screenshot-1-l.png) |
| 🔍 **Search results** | 🔐 **Sign in** |
| ![Search](screenshots/shopcrawl-productsearch-screenshot-1-l.png) | ![Login](screenshots/shopcrawl-login-screenshot-l.png) |

<details>
<summary>📱 <b>Mobile views</b></summary>

| Home | Search | SmartRank |
|:---:|:---:|:---:|
| ![](screenshots/shopcrawl-home-screenshot-m.png) | ![](screenshots/shopcrawl-productsearch-screenshot-m.png) | ![](screenshots/shopcrawl-smartrank-screenshot-2-m.png) |

</details>

## 🧮 How SmartRank™ picks a winner

Every store offering a product gets a score out of 100:

```js
score = 0.45 × costScore     // cheapest (price + shipping) ÷ this store's total
      + 0.35 × trustScore    // store rating out of 10
      + 0.20 × speedScore    // fastest delivery ÷ this store's delivery days

if (rating < 6.0) score *= 0.8   // 🚩 risk penalty: cheap is useless if it never arrives
```

The table then shows each store's total cost in KES, its shipping time, a star rating and a penalty flag, with the winner on top.

## ✨ Features

- 🔍 **One search bar, four stores**, backed by the `?search=` API
- 🏆 **SmartRank™ comparison table**: total cost, delivery speed and trust in one view
- 📜 **Recently viewed timeline**: your last 11 products, synced to your account
- 🔐 **Sign up / sign in / PIN-based password reset**
- 🛡️ **Admin dashboard**: add, edit and delete products (server-enforced)
- 📱 **Mobile-first**, with toast notifications for every action

## 🚀 Run it locally

```bash
git clone https://github.com/JessyWaweru/shopcrawl-web.git
cd shopcrawl-web
npm install
npm start                 # → http://localhost:3000
```

To use a local backend, switch `API_URL` in [`src/config.js`](src/config.js) to `http://127.0.0.1:8000` and run [shopcrawl-api](https://github.com/JessyWaweru/shopcrawl-api).

---

<div align="center">

**Built by Jessy Bryan Waweru**: actuary by training, full-stack engineer by obsession.

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?logo=linkedin&logoColor=white)](https://www.linkedin.com/in/jessy-waweru-b8051a288)
[![Email](https://img.shields.io/badge/Email-EA4335?logo=gmail&logoColor=white)](mailto:bryanjessywaweru@gmail.com)
[![GitHub](https://img.shields.io/badge/More_projects-181717?logo=github)](https://github.com/JessyWaweru)

</div>
