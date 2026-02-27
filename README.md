# Luchiano Wireless Website

Official website for Luchiano Wireless - Phones, Repairs, Activations & Africa Shipping.

**Live Site:** [luchianowireless.com](https://luchianowireless.com)

---

## 🚀 Quick Setup

### 1. Deploy to Netlify (FREE)

```bash
# Already pushed to GitHub
# Just connect Netlify to this repo
```

**Steps:**
1. Go to [netlify.com](https://netlify.com) → Sign up (free)
2. Click "Add new site" → "Import from GitHub"
3. Select `Louch84/luchiano-wireless-site`
4. Build settings:
   - **Build command:** *(leave empty)*
   - **Publish directory:** `/` (root)
5. Click "Deploy site"

### 2. Connect Your Domain

1. In Netlify: **Site settings** → **Domain management**
2. Click "Add custom domain"
3. Enter: `luchianowireless.com`
4. Netlify shows DNS records
5. Go to your domain registrar → Update DNS to point to Netlify

**DNS Records:**
```
Type: A
Name: @
Value: 75.2.60.5
```

---

## 🛠️ Customization

### Update Contact Info

Edit `index.html` - search for `YOUR_NUMBER` and replace with your actual WhatsApp number:

```html
<!-- Line ~15 -->
<a href="https://wa.me/12155551234" class="btn btn-whatsapp">

<!-- Line ~150 -->
<a href="https://wa.me/12155551234" class="btn btn-primary btn-large">
```

### Add Real Products

Edit `index.html` - find the `.product-card` sections and update:

```html
<div class="product-card">
    <div class="product-image">
        <span class="condition-badge clean">Clean IMEI</span>
        <img src="your-photo.jpg" alt="iPhone 14 Pro">
    </div>
    <div class="product-info">
        <h3>iPhone 14 Pro</h3>
        <p class="specs">256GB • Deep Purple • 92% Battery</p>
        <div class="product-price">
            <span class="price">$699</span>
        </div>
        <a href="https://tally.so/r/YOUR_FORM_ID" class="btn btn-small">Order Now</a>
    </div>
</div>
```

### Connect Tally Forms

1. Go to [tally.so](https://tally.so) → Create free account
2. Create forms using templates in `TALLY_FORMS.md`
3. Get form URL (e.g., `tally.so/r/abc123`)
4. Replace `YOUR_FORM_ID` in `index.html` with your actual form IDs

---

## 📱 WhatsApp Business Setup

See `WHATSAPP_TEMPLATES.md` for complete setup guide including:

- Quick reply shortcuts
- Automated greeting/away messages
- Product catalog templates
- Payment collection scripts

**Quick Start:**
1. Download WhatsApp Business app (free)
2. Set up business profile
3. Add quick replies from `WHATSAPP_TEMPLATES.md`
4. Create product catalog

---

## 📁 File Structure

```
luchiano-wireless-site/
├── index.html                    # Main website
├── styles.css                    # Styles (dark theme)
├── README.md                     # This file
├── TALLY_FORMS.md                # Order form templates
└── WHATSAPP_TEMPLATES.md         # WhatsApp scripts
```

---

## 🔄 Updates

To update the website:

```bash
# Edit files
# Then commit and push
git add .
git commit -m "Update product prices"
git push origin main

# Netlify auto-deploys on push
```

---

## 💰 Costs

| Service | Cost |
|---------|------|
| Netlify Hosting | FREE |
| Tally Forms | FREE (unlimited) |
| WhatsApp Business | FREE |
| Domain (you own) | FREE |
| **Total** | **$0/month** |

**Transaction fees:**
- Stripe: 2.9% + 30¢ per transaction (if you add Stripe later)
- CashApp/Venmo: FREE for personal, 1.5% for business
- Mobile Money: Varies by provider

---

## 🎨 Customization Options

### Change Colors

Edit `styles.css` - update the color variables:

```css
:root {
    --primary: #6366f1;      /* Main brand color */
    --primary-dark: #4f46e5; /* Hover state */
    --accent: #f59e0b;       /* Highlights/badges */
}
```

### Add More Pages

Create new HTML files:

```bash
# Example: repairs.html
cp index.html repairs.html
# Edit content for repairs page
# Add link in navigation
```

### Add Analytics

Add Google Analytics or similar:

```html
<!-- Add to <head> in index.html -->
<script async src="https://www.googletagmanager.com/gtag/js?id=GA_MEASUREMENT_ID"></script>
```

---

## 📞 Support

For issues or questions:
- WhatsApp: [Your Number]
- Email: info@luchianowireless.com

---

## 📝 Next Steps

1. [ ] Deploy to Netlify
2. [ ] Connect luchianowireless.com domain
3. [ ] Create Tally forms (use TALLY_FORMS.md)
4. [ ] Set up WhatsApp Business (use WHATSAPP_TEMPLATES.md)
5. [ ] Add real product photos
6. [ ] Update contact info throughout
7. [ ] Test order flow end-to-end
8. [ ] Launch!

---

**Built with:** HTML, CSS, ❤️  
**License:** Proprietary - Luchiano Wireless
