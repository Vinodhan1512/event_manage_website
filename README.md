# Chennai Event Management Website

A professional, modern, and mobile-friendly website for an Event Management Company built with HTML5, CSS3, and JavaScript.

## Features

- **Responsive Design**: Mobile-first approach that works seamlessly on all devices
- **Modern UI**: Clean, professional design with vibrant colors matching the brand
- **Interactive Elements**:
  - Auto-sliding hero carousel
  - Image lightbox for portfolio
  - Smooth scrolling navigation
  - Form validation
  - Animated elements on scroll
- **Contact Options**:
  - Floating WhatsApp and Call buttons
  - Contact form with validation
  - Multiple contact methods
- **SEO Optimized**: Semantic HTML and meta tags for better search visibility

## Pages

1. **Home (index.html)**: Welcome page with services overview and portfolio preview
2. **Services (services.html)**: Detailed list of all event planning services
3. **Portfolio (portfolio.html)**: Gallery of past events with testimonials
4. **About Us (about.html)**: Company information, mission, vision, and achievements
5. **Contact (contact.html)**: Contact form, business hours, and FAQ

## Directory Structure

```
event_manage_website/
├── index.html
├── services.html
├── portfolio.html
├── about.html
├── contact.html
├── css/
│   └── style.css
├── js/
│   └── script.js
├── images/
│   ├── logo.png (Add your logo here)
│   ├── hero1.jpg
│   ├── hero2.jpg
│   ├── hero3.jpg
│   ├── event1.jpg through event12.jpg
│   └── ... (Add your event photos)
└── README.md
```

## Adding Your Images

To personalize the website with your own images:

1. **Logo**: Add your company logo as `images/logo.png` (recommended size: 200x200px)
2. **Hero Images**: Add 3 hero slider images as:
   - `images/hero1.jpg` - Corporate event (1920x1080px recommended)
   - `images/hero2.jpg` - Wedding event (1920x1080px recommended)
   - `images/hero3.jpg` - Conference event (1920x1080px recommended)
3. **Portfolio Images**: Add event photos as:
   - `images/event1.jpg` through `images/event12.jpg` (800x600px recommended)

**Note**: If images are not added, the website will display placeholder images automatically.

## Customization

### Update Contact Information

Edit the following in **all HTML files**:

1. **Phone Numbers**: Replace `+919876543210` with your actual phone number
2. **Email Addresses**: Replace `info@chennaieventmanagement.com` with your actual email
3. **WhatsApp Link**: Update `https://wa.me/919876543210` with your WhatsApp number
4. **Address**: Update "Chennai, Tamil Nadu" with your actual address

### Update Colors

Edit `css/style.css` to change the color scheme:

```css
:root {
    --primary-color: #FF6B35;      /* Orange */
    --secondary-color: #F7931E;    /* Yellow-Orange */
    --accent-purple: #8B5CF6;      /* Purple */
    --accent-pink: #EC4899;        /* Pink */
}
```

### Update Social Media Links

In the footer section of each HTML file, replace `#` with your actual social media URLs:

```html
<a href="YOUR_FACEBOOK_URL" aria-label="Facebook"><i class="fab fa-facebook"></i></a>
<a href="YOUR_INSTAGRAM_URL" aria-label="Instagram"><i class="fab fa-instagram"></i></a>
```

## GitHub Pages Deployment

### Step 1: Verify Branch

Make sure you're on the correct branch:

```bash
git branch
```

You should see `claude/check-website-access-frDSG` marked with an asterisk.

### Step 2: Push to GitHub

```bash
# Add all files
git add .

# Commit changes
git commit -m "Add complete event management website"

# Push to GitHub
git push -u origin claude/check-website-access-frDSG
```

### Step 3: Enable GitHub Pages

1. Go to your GitHub repository
2. Click on **Settings**
3. Scroll down to **Pages** section
4. Under "Source", select the branch: `claude/check-website-access-frDSG`
5. Select folder: `/ (root)`
6. Click **Save**

Your site will be published at: `https://YOUR_USERNAME.github.io/event_manage_website/`

### Step 4: Custom Domain (Optional)

To use a custom domain like `chennaieventmanagementservice.com`:

1. In GitHub Pages settings, add your custom domain
2. In your domain registrar (GoDaddy, Namecheap, etc.), add these DNS records:

```
Type: A
Name: @
Value: 185.199.108.153
       185.199.109.153
       185.199.110.153
       185.199.111.153

Type: CNAME
Name: www
Value: YOUR_USERNAME.github.io
```

3. Create a file named `CNAME` in the repository root with your domain:
```
chennaieventmanagementservice.com
```

## Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)
- Mobile browsers (iOS Safari, Chrome Mobile)

## Technologies Used

- **HTML5**: Semantic markup
- **CSS3**: Flexbox, Grid, Animations, Media Queries
- **JavaScript**: Vanilla JS (no frameworks)
- **Font Awesome 6.4.0**: Icons
- **Google Fonts**: System fonts for faster loading

## Performance

- Mobile-first responsive design
- Optimized images with fallback placeholders
- Minimal external dependencies
- Fast loading times
- SEO optimized

## Support

For any issues or customization needs, contact:
- Email: info@chennaieventmanagement.com
- Phone: +91 98765 43210

## License

© 2024 Chennai Event Management. All rights reserved.

---

## Quick Start Checklist

- [ ] Add your logo to `images/logo.png`
- [ ] Add hero images (hero1.jpg, hero2.jpg, hero3.jpg)
- [ ] Add portfolio event images (event1.jpg through event12.jpg)
- [ ] Update phone numbers in all HTML files
- [ ] Update email addresses in all HTML files
- [ ] Update WhatsApp link with your number
- [ ] Update physical address
- [ ] Add social media links
- [ ] Test website locally
- [ ] Push to GitHub
- [ ] Enable GitHub Pages
- [ ] Test live website
- [ ] (Optional) Set up custom domain

## Local Development

To test the website locally:

1. Simply open `index.html` in your web browser
2. Or use a local server:
   ```bash
   # Using Python 3
   python -m http.server 8000

   # Using PHP
   php -S localhost:8000

   # Using Node.js (with http-server)
   npx http-server
   ```
3. Navigate to `http://localhost:8000`

## Future Enhancements

- Add Google Maps integration
- Add blog section
- Integrate contact form with backend
- Add gallery filtering
- Add live chat widget
- Add event booking system
- Add client testimonials slider
- Multilingual support (Tamil/English)
