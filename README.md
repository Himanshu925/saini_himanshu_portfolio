README
======

# Himanshu Saini - Portfolio Website 🚀

Professional portfolio website showcasing web design and development skills, projects, and certifications.

## ✨ Features

- **Responsive Design** - Works perfectly on desktop, tablet, and mobile devices
- **Dark/Light Mode** - Toggle between themes for better viewing
- **Virtual Assistant Chat** - Interactive AI chatbot with predefined Q&A
- **WhatsApp Direct Chat** - Quick messaging integration with WhatsApp
- **Admin Dashboard** - Secure login system to manage contact forms and chat logs
- **Certificate Section** - Display professional certifications and credentials
- **Skills Showcase** - Interactive skill bars for HTML, CSS, JavaScript, UI/UX, React
- **Social Media Integration** - Links to Instagram, Twitter, LinkedIn, YouTube
- **Contact Form** - Integrated contact form with Formspree
- **SEO Optimized** - Meta tags and structured data for search engines
- **Google AdSense** - Monetization support

## 🛠️ Tech Stack

**Frontend:**
- HTML5, CSS3, JavaScript
- Bootstrap 5.3.0
- Font Awesome Icons
- AOS (Animate On Scroll)

**Backend:**
- Node.js & Express.js
- MongoDB (optional - for contact/chat storage)
- Body Parser, CORS

**Hosting Options:**
- Netlify (Recommended for frontend)
- Vercel (Alternative)
- Heroku (For full-stack)
- AWS, DigitalOcean, Render

## 📋 Requirements

- Node.js v14+

> 🟢 Triggering redeploy: This repository is configured to auto-deploy via Vercel. If you are not seeing changes, refresh the Vercel deployment dashboard and/or clear your browser cache.
 
- npm or yarn
- MongoDB (optional)

## 🚀 Local Setup

### 1. Clone or Download
```bash
git clone <your-repo-url>
cd insta
```

### 2. Install Dependencies
```bash
npm install
```

### 3. Configure MongoDB (Optional)
Edit `server.js` and update MongoDB URI:
```javascript
const mongoURI = 'mongodb://localhost:27017/portfolio';
```

Or use MongoDB Atlas:
```javascript
const mongoURI = 'mongodb+srv://username:password@cluster.mongodb.net/portfolio';
```

### 4. Run Locally
```bash
npm start
```
Server runs on `http://localhost:3000`

### 5. Development Mode (with auto-reload)
```bash
npm run dev
```

## 🔐 Admin Credentials

Located in `server.js` comments:
- **Username:** `admin_himanshu`
- **Password:** `portfolio2025!secure`

⚠️ **IMPORTANT:** Change these credentials before deployment!

## 📱 WhatsApp Integration

Your WhatsApp number is already configured: **+91 7906156268**

To change:
1. Edit all `.html` files
2. Replace `https://wa.me/917906156268` with your WhatsApp link
3. Format: `https://wa.me/+[COUNTRY_CODE][NUMBER]`

## 📝 Contact Form Configuration

Currently uses **Formspree** for email delivery.

Update in `index.html`:
```javascript
fetch('https://formspree.io/f/mgolrqqk', {
```

To set up your own:
1. Go to formspree.io
2. Create account and form
3. Get your form ID
4. Replace in the JavaScript code

## 📤 Deployment Options

### Option 1: Netlify (Recommended - Frontend Only)

1. **Build:**
```bash
# No build needed - static files
```

2. **Deploy:**
   - Go to netlify.com
   - Connect GitHub repository
   - Set build command: `npm install`
   - Set publish directory: `./`
   - Deploy!

3. **Environment Variables:**
   - Not needed for static deployment

### Option 2: Vercel (Frontend Only)

1. **Deploy:**
   - Go to vercel.com
   - Import GitHub project
   - Click "Deploy"
   - Done!

### Option 3: Heroku (Full Stack with Backend)

1. **Create app:**
```bash
heroku login
heroku create your-app-name
```

2. **Set MongoDB URI:**
```bash
heroku config:set MONGODB_URI="your_mongodb_atlas_url"
```

3. **Deploy:**
```bash
git push heroku main
```

### Option 4: DigitalOcean App Platform

1. Connect GitHub repository
2. Configure build settings
3. Set environment variables
4. Deploy!

### Option 5: Render.com

1. Go to render.com
2. Click "New +"
3. Select "Web Service"
4. Connect GitHub
5. Configure and deploy

### Option 6: AWS EC2

1. Launch EC2 instance
2. Install Node.js and npm
3. Clone repository
4. Install dependencies
5. Set up MongoDB
6. Use PM2 to run server
7. Set up Nginx as reverse proxy
8. Configure SSL with Let's Encrypt

## 🔒 Security Checklist

Before deployment:
- [ ] Change admin credentials in `server.js`
- [ ] Update MongoDB connection string
- [ ] Update Formspree form ID
- [ ] Enable HTTPS
- [ ] Set up security headers
- [ ] Configure CORS properly
- [ ] Use environment variables for sensitive data
- [ ] Add .gitignore file
- [ ] Review all external links

## 🌐 Domain Setup

1. Buy domain from Namecheap, GoDaddy, or Bluehost
2. Point nameservers to your hosting provider
3. Update DNS records as per provider instructions
4. Wait 24-48 hours for propagation

## 📊 Performance Tips

- Compress images using TinyPNG or ImageOptim
- Enable Gzip compression
- Use CDN for static files
- Minify CSS and JavaScript
- Implement caching strategies
- Use lazy loading for images

## 🐛 Troubleshooting

**Port 3000 already in use:**
```bash
# Find process using port 3000
netstat -ano | findstr :3000

# Kill process (Windows)
taskkill /PID [PID] /F

# Or use different port
PORT=3001 npm start
```

**MongoDB connection error:**
- Verify MongoDB is running
- Check connection string
- Verify IP whitelist in MongoDB Atlas

**WhatsApp links not working:**
- Test on actual WhatsApp
- Ensure number format is correct with country code
- Check internet connection

**Contact form not working:**
- Check Formspree form ID
- Verify form ID in index.html
- Test email address

## 📈 Analytics & Monitoring

Add Google Analytics:
```html
<!-- Add to <head> tag -->
<script async src="https://www.googletagmanager.com/gtag/js?id=GA_ID"></script>
```

## 📞 Support & Contact

- **Email:** sainihimanshu27958@gmail.com
- **WhatsApp:** +91 7906156268
- **GitHub:** [Your GitHub Profile]
- **LinkedIn:** [Your LinkedIn Profile]

## 📄 License

ISC License - Feel free to use this project!

## 🙏 Credits

- Bootstrap 5.3.0
- Font Awesome Icons
- AOS (Animate On Scroll)
- Formspree (Contact Form)
- MongoDB (Database)

---

**Last Updated:** March 18, 2026
**Version:** 1.0.0
**Status:** ✅ Fully Tested & Ready for Production