# Balya Vardhan Gurukul — School Website

## 🚀 Deploy to Vercel in 3 steps

1. Upload this folder to a **GitHub repository**
2. Go to [vercel.com](https://vercel.com) → **New Project** → Import your repo
3. Hit **Deploy** — no build settings needed (static HTML)

Your site will be live at `https://your-project-name.vercel.app`

---

## 📁 Project Structure

```
balya-vardhan-gurukul/
├── index.html        ← The entire website (single file)
├── vercel.json       ← Vercel routing config
├── public/
│   └── logo.png      ← School logo (already placed)
└── README.md
```

---

## ✏️ How to Update Content

All content is inside `index.html`. Search for these placeholders to update:

| What to change | Search for |
|---|---|
| Phone number | `+91 12345 67890` |
| Email | `info@balyavardhan.edu.in` |
| Address | `Plot No. 45, Sector 14, Vasundhara` |
| Google Maps link | `maps.google.com/?q=Vasundhara` |
| Social media links | `href="#" title="Facebook"` etc. |
| Admission dates | `Forms Available`, `Session Begins` |
| Stats (students, teachers) | `500+`, `30+`, `10+` |

## 🖼️ Adding Real Photos (Gallery)

Replace the emoji `gallery-item` divs with:
```html
<div class="gallery-item">
  <img src="public/gallery/photo1.jpg" alt="..." style="width:100%;height:100%;object-fit:cover;" />
  <div class="caption">Caption Here</div>
</div>
```

## 📞 Connect a Real Form

The enquiry forms currently show a toast message. To get real email notifications, integrate with:
- **Formspree** (free): replace `submitForm()` with a `fetch` POST to `https://formspree.io/f/your-id`
- **EmailJS**: free email sending from JavaScript
- **Google Forms**: embed a Google Form in the `#admissions` section

## 🗺️ Embed Real Google Maps

1. Go to [maps.google.com](https://maps.google.com)
2. Search your school location → Share → Embed a map → Copy iframe
3. Replace the `.map-placeholder` div with the iframe

---

Built with ❤️ for Balya Vardhan Gurukul
