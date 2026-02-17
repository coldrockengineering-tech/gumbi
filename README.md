# Farmerz Market - Netlify Ready Website

This is a complete, production-ready static website for Farmerz Market that works perfectly on Netlify.

## 📁 File Structure

```
netlify_site/
├── index.html          # Main HTML file
├── css/
│   └── style.css       # All styling
├── js/
│   └── script.js       # All JavaScript functionality
├── images/             # Product and content images
│   └── placeholder.txt  # Image naming guide
└── README.md           # This file
```

## 🚀 How to Deploy to Netlify

### Method 1: Drag & Drop (Easiest)

1. Go to [Netlify.com](https://netlify.com)
2. Sign up or log in
3. Drag and drop the entire `netlify_site` folder onto Netlify
4. Your site will be live in seconds!

### Method 2: GitHub Integration

1. Create a GitHub repository named `somkhandas`
2. Upload all files to the repository
3. Connect GitHub to Netlify
4. Netlify will auto-deploy on every push

### Method 3: Netlify CLI

```bash
# Install Netlify CLI
npm install -g netlify-cli

# Deploy
netlify deploy --prod --dir .
```

## 📸 Adding Product Images

The website includes placeholders for images. To add your actual product photos:

1. Replace files in the `images/` folder:
   - `hero-meat.jpg` - Hero section image
   - `combo-1.jpg` - Combo package image
   - `beef-stew.jpg`, `beef-chuck.jpg`, etc. - Individual product images

2. Keep the exact filenames
3. Use JPG format for best performance
4. Recommended sizes:
   - Hero: 600x400px
   - Combos: 400x300px
   - Products: 300x300px

**Note:** If images are missing, the site will display placeholder SVG graphics, so you can deploy first and add images later.

## ✨ Features Included

✅ Sticky navigation header with logo and call button
✅ Hero section with business name and tagline
✅ About section with farm information
✅ Core values section
✅ Premium combo packages (5 combos)
✅ Individual products (12 products with images + 4 text-only products)
✅ Quotation request form
✅ Contact section with payment and delivery info
✅ WhatsApp floating button
✅ Mobile responsive design
✅ Cart counter with localStorage
✅ Smooth scrolling navigation
✅ Toast notifications
✅ Fully accessible

## 🎨 Customization

### Change Colors

Edit the CSS variables in `css/style.css`:

```css
:root {
    --primary-color: #6B3E3E;      /* Burgundy */
    --secondary-color: #dc143c;    /* Red */
    --accent-color: #D4A574;       /* Gold */
    /* ... more colors ... */
}
```

### Update Business Info

Edit in `index.html`:
- Phone number: Search for `+27688359960`
- Email: Search for `info@somkhandas.co.za`
- Address: Search for `Arcadia, Pretoria`
- Bank details: Search for `Bidvest Bank`

### Add/Remove Products

Edit the product sections in `index.html`:
- Combo packages: Look for `combos-grid` section
- Individual products: Look for `products-grid-featured` section

## 📱 Mobile Responsive

The website is fully responsive and works perfectly on:
- Desktop (1200px+)
- Tablet (768px - 1199px)
- Mobile (480px - 767px)
- Small mobile (<480px)

## 🔧 Technical Details

- **No dependencies** - Pure HTML, CSS, JavaScript
- **No build process** - Deploy as-is
- **Fast loading** - Optimized CSS and JavaScript
- **SEO friendly** - Proper meta tags and semantic HTML
- **Accessible** - WCAG compliant with keyboard navigation
- **Cross-browser** - Works on all modern browsers

## 📞 Contact Integration

### WhatsApp Button
- Located at bottom-right of screen
- Automatically opens WhatsApp chat with your number
- Edit the number in `index.html`: `href="https://wa.me/27688359960"`

### Contact Form
- Quotation form validates all fields
- Shows success/error messages
- Data can be sent to WhatsApp or email backend

### Phone Links
- Click-to-call buttons throughout the site
- Edit phone number: `href="tel:+27688359960"`

## 🌐 Domain Setup

After deploying to Netlify:

1. Go to Site Settings
2. Click "Domain management"
3. Add your custom domain or use the Netlify subdomain

## 📊 Analytics (Optional)

To add Google Analytics:

1. Add this before `</head>` in `index.html`:
```html
<!-- Google Analytics -->
<script async src="https://www.googletagmanager.com/gtag/js?id=YOUR_GA_ID"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());
  gtag('config', 'YOUR_GA_ID');
</script>
```

2. Replace `YOUR_GA_ID` with your Google Analytics ID

## 🐛 Troubleshooting

### Images not showing
- Check image filenames match exactly
- Ensure images are in the `images/` folder
- Try refreshing the page (Ctrl+F5)

### Styles not loading
- Clear browser cache
- Check that `css/style.css` path is correct
- Verify file permissions

### JavaScript not working
- Check browser console for errors (F12)
- Ensure `js/script.js` path is correct
- Try a different browser

## 📝 License

This website is created for Farmerz Market. All rights reserved.

## 🎯 Next Steps

1. Deploy to Netlify
2. Add your product images
3. Set up custom domain
4. Add Google Analytics
5. Test on mobile devices
6. Share with customers!

---

**Need help?** Contact Netlify support or visit [Netlify Docs](https://docs.netlify.com)
