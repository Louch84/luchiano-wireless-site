# Product Image Sources - Luchiano Wireless

## ✅ Free Image Sources (No Copyright Issues)

### Option 1: Placeholder Images (CURRENT - Works Now)
Using placehold.co - reliable, fast, no hotlinking issues

**Format:**
```
https://placehold.co/300x400/1a1a1a/ffffff?text=iPhone+15+Pro
```

**Colors by Brand:**
- iPhone: `#1a1a1a` (dark gray)
- Samsung: `#2d2d2d` (medium gray)
- Budget phones: `#3d3d3d` (light gray)

---

### Option 2: PNGTree (Free with Attribution)
**URL:** https://pngtree.com/

**Search Terms:**
- "iPhone 15 Pro PNG"
- "iPhone 14 Pro Max transparent"
- "Samsung S23 PNG"
- "Smartphone mockup"

**Note:** Requires free account, some daily download limits

---

### Option 3: Unsplash (Free, No Attribution Required)
**URL:** https://unsplash.com/s/photos/iphone

**Direct Image URLs (Hotlink-Friendly):**
```
https://images.unsplash.com/photo-1696446702022-0af1fbb4227b?w=400 (iPhone 15)
https://images.unsplash.com/photo-1678652197831-2d180705cd2c?w=400 (iPhone 14)
https://images.unsplash.com/photo-1632661674526-e5e546388810?w=400 (iPhone 13)
```

---

### Option 4: Pexels (Free, No Attribution)
**URL:** https://www.pexels.com/search/iphone/

**Good for:** Lifestyle shots, phones in hand, real-world use

---

### Option 5: Generate Your Own (BEST FOR CONSISTENCY)

**Setup:**
1. Get a phone stand ($20 Amazon)
2. Use white poster board as background ($5)
3. Natural light or ring light ($30)
4. Use your phone camera
5. Remove background with remove.bg (free)

**Process:**
1. Photograph each phone (front + back)
2. Upload to remove.bg → transparent PNG
3. Save to `luchiano-wireless-site/images/` folder
4. Update HTML with real images

---

## 📸 Quick Image Grab Script

Create this script to download images:

```python
# download_images.py
import requests
import os

# Create images folder
os.makedirs('images', exist_ok=True)

# Image URLs (replace with actual URLs)
images = {
    'iphone-15-pro.png': 'https://example.com/iphone15pro.png',
    'iphone-14-pro-max.png': 'https://example.com/iphone14promax.png',
    # Add more...
}

for filename, url in images.items():
    response = requests.get(url)
    with open(f'images/{filename}', 'wb') as f:
        f.write(response.content)
    print(f'Downloaded {filename}')
```

---

## 🎨 Recommended: Use Placeholders for Now

**Why:**
- ✅ Works immediately (no downloads)
- ✅ Fast loading
- ✅ No copyright issues
- ✅ Consistent sizing
- ✅ Can customize text/colors

**Upgrade Later:**
Once you're making sales, invest 2-3 hours photographing your actual inventory. Real photos convert better!

---

## 📋 Image Checklist for Each Product

When photographing:
- [ ] Front view (screen on, showing wallpaper)
- [ ] Back view (showing color, camera)
- [ ] Side view (showing condition)
- [ ] Any damage clearly photographed
- [ ] IMEI screen (for verification)
- [ ] Battery health screenshot

**File Naming:**
```
iphone-15-pro-128gb-natural-front.png
iphone-15-pro-128gb-natural-back.png
iphone-14-pro-max-256gb-purple-front.png
```

---

## 🔗 Current Site Images

All products currently using:
```
https://placehold.co/300x400/1a1a1a/ffffff?text=iPhone+15+Pro
```

**To Update:**
1. Take/download real photos
2. Save to `luchiano-wireless-site/images/`
3. Replace image URLs in HTML:
   ```html
   <!-- OLD -->
   <img src="https://placehold.co/300x400/..." alt="iPhone 15 Pro">
   
   <!-- NEW -->
   <img src="images/iphone-15-pro.png" alt="iPhone 15 Pro">
   ```
4. Commit and push to GitHub

---

**Priority:** 
1. Get placeholder site working first ✅
2. Start selling
3. Photograph top 20 sellers
4. Update site gradually

Don't let perfect be the enemy of profitable!
