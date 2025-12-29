# GitHub Pages Deployment Instructions

## Quick Start - Enable GitHub Pages

Follow these steps to make your website live on GitHub Pages:

### Step 1: Access Repository Settings

1. Go to your GitHub repository: https://github.com/Vinodhan1512/event_manage_website
2. Click on the **Settings** tab (top right area of the page)

### Step 2: Navigate to Pages Settings

1. In the left sidebar, scroll down and click on **Pages**
2. You should now see the "GitHub Pages" configuration section

### Step 3: Configure Source

1. Under **"Build and deployment"** section:
   - **Source**: Select "Deploy from a branch"
   - **Branch**: Select `claude/check-website-access-frDSG`
   - **Folder**: Select `/ (root)`
2. Click the **Save** button

### Step 4: Wait for Deployment

1. GitHub will start building your site (this takes 1-2 minutes)
2. Refresh the page after a minute
3. You'll see a message: "Your site is live at https://vinodhan1512.github.io/event_manage_website/"

### Step 5: Visit Your Website

Your website will be available at:
**https://vinodhan1512.github.io/event_manage_website/**

---

## Setting Up Custom Domain (Optional)

If you want to use your own domain like `chennaieventmanagementservice.com`:

### Step 1: Add Domain in GitHub

1. Go to Settings > Pages
2. Under "Custom domain", enter: `chennaieventmanagementservice.com`
3. Click **Save**

### Step 2: Configure DNS Records

In your domain registrar (GoDaddy, Namecheap, etc.), add these DNS records:

#### For Root Domain (chennaieventmanagementservice.com):

```
Type: A
Name: @ (or leave blank)
Value: 185.199.108.153
TTL: 3600

Type: A
Name: @
Value: 185.199.109.153
TTL: 3600

Type: A
Name: @
Value: 185.199.110.153
TTL: 3600

Type: A
Name: @
Value: 185.199.111.153
TTL: 3600
```

#### For WWW Subdomain:

```
Type: CNAME
Name: www
Value: vinodhan1512.github.io
TTL: 3600
```

### Step 3: Create CNAME File

Create a file named `CNAME` (no extension) in your repository root with content:
```
chennaieventmanagementservice.com
```

Commit and push this file.

### Step 4: Enable HTTPS (Recommended)

1. After DNS propagates (24-48 hours), go back to Settings > Pages
2. Check the box: **Enforce HTTPS**
3. Your site will now use HTTPS (secure connection)

---

## Next Steps After Deployment

### 1. Add Your Images

Replace placeholder images with your actual event photos:

```
images/
├── logo.png          (Your company logo)
├── hero1.jpg         (Corporate event photo)
├── hero2.jpg         (Wedding event photo)
├── hero3.jpg         (Conference photo)
├── event1.jpg        (Portfolio image 1)
├── event2.jpg        (Portfolio image 2)
... (up to event12.jpg)
```

**How to add images:**
1. Click on the `images` folder in GitHub
2. Click "Add file" > "Upload files"
3. Drag and drop your images
4. Commit the changes

### 2. Update Contact Information

Update these in all HTML files (index.html, services.html, etc.):

- Phone number: `+919876543210` → Your actual phone
- Email: `info@chennaieventmanagement.com` → Your actual email
- WhatsApp: `https://wa.me/919876543210` → Your WhatsApp number
- Address: Add your complete address

**How to edit files on GitHub:**
1. Click on any HTML file
2. Click the pencil icon (Edit this file)
3. Make your changes
4. Click "Commit changes"

### 3. Add Social Media Links

In the footer of each HTML file, replace `#` with your social media URLs:

```html
<a href="https://facebook.com/yourpage">Facebook</a>
<a href="https://instagram.com/yourhandle">Instagram</a>
```

### 4. Test Your Website

1. Open your website URL
2. Test on mobile device (or use browser dev tools)
3. Test all navigation links
4. Test the contact form
5. Check WhatsApp and Call buttons work

---

## Troubleshooting

### Website Not Showing Up?

- Wait 2-3 minutes after enabling GitHub Pages
- Hard refresh your browser (Ctrl+Shift+R or Cmd+Shift+R)
- Check that the branch name is correct: `claude/check-website-access-frDSG`

### Custom Domain Not Working?

- DNS changes can take 24-48 hours to propagate
- Use https://dnschecker.org to verify DNS records
- Make sure CNAME file exists in repository root
- Ensure DNS records are correctly configured at your registrar

### Images Not Showing?

- Check file names match exactly (case-sensitive)
- Ensure images are in the `images/` folder
- Verify image formats are supported (.jpg, .png, .gif)

### Making Changes After Deployment?

Any changes you push to the `claude/check-website-access-frDSG` branch will automatically deploy to GitHub Pages within 1-2 minutes.

---

## Support

If you need help:
1. Check the main README.md file
2. Visit GitHub Pages documentation: https://docs.github.com/pages
3. Check your repository's Actions tab for deployment status

---

## Current Status

✅ Website code created and pushed to GitHub
✅ Branch: `claude/check-website-access-frDSG`
⏳ Next step: Enable GitHub Pages (follow Step 1-5 above)

**Your repository URL:**
https://github.com/Vinodhan1512/event_manage_website

**After enabling GitHub Pages, your site will be at:**
https://vinodhan1512.github.io/event_manage_website/
