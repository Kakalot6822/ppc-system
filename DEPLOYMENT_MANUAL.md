# PPC System - Manual Deployment

## Quick Start (5 minutes)

### Automatic Deployment via Vercel UI
1. Go to https://vercel.com/new
2. Connect GitHub account
3. Import repository
4. Click Deploy
5. Get live URL instantly

### Command Line Deployment
```bash
npm i -g vercel
vercel login
vercel --prod
```

## Manual File Upload

### Using GitHub Web UI
1. Go to https://github.com/Kakalot6822/ppc-system
2. Click "Add file" > "Create new file"
3. Add files:
   - index.html
   - dashboard.html
   - style.css
   - script.js

### Using Git Command Line
```bash
git clone https://github.com/Kakalot6822/ppc-system.git
cd ppc-system
git add .
git commit -m "Add project files"
git push origin main
```

## Environment Setup

### Local Development
- No build process needed!
- Just open index.html in browser

### Production
- Automatically deployed by Vercel
- No environment variables required
- No database setup needed

## Customization

### Change Admin Email
Edit dashboard.html:
```html
<p>Email: <strong>your-email@gmail.com</strong></p>
```

### Change Commission Rate
Modify script.js:
```javascript
const COMMISSION_RATE = 299;
```

## Monitoring

1. Visit https://vercel.com/dashboard
2. Click `ppc-system` project
3. View deployment history
4. Monitor logs and performance

## Troubleshooting

- Blank page? Check browser console (F12)
- 404 error? Verify file names
- Styling missing? Check style.css link
- Deployment stuck? Retry from dashboard

## File Checklist

- [ ] index.html
- [ ] dashboard.html
- [ ] style.css
- [ ] script.js
- [ ] DEPLOYMENT_SUMMARY.md
- [ ] DEPLOYMENT_PACKAGE.md
- [ ] DEPLOYMENT_MANUAL.md

## Security Notes

- Avoid hardcoding sensitive data
- Use environment variables for secrets
- HTTPS enabled automatically with Vercel
- Regular security audits recommended

## Next Steps

1. Test all 8 features
2. Monitor performance
3. Update documentation
4. Plan future enhancements
