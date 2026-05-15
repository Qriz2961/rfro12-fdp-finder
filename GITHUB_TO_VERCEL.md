# GitHub → Vercel Deployment Checklist

## Files to Upload to GitHub

**Rename and upload these 3 files:**

| File | Rename To | Purpose |
|------|-----------|---------|
| `index-hybrid.html` | `index.html` | The complete web app |
| `sample-data.csv` | `sample-data.csv` | Data format example |
| `README.md` | `README.md` | Documentation (optional) |

**Do NOT upload:**
- Old index.html
- Other .md files
- .gitignore
- Any other files

---

## GitHub Setup (5 minutes)

### 1️⃣ Create GitHub Account (if needed)
- Go to: https://github.com/signup
- Email, password, username
- Verify email

### 2️⃣ Create Repository
- Go to: https://github.com/new
- **Name:** `rfro12-fdp-gas-station-finder`
- **Description:** `RFRO XII Fuel Discount Program Gas Station Finder`
- **Public:** ✓ (checked)
- Click "Create repository"

### 3️⃣ Upload Files
- Click "Add file" → "Upload files"
- Select 3 files (with index.html renamed)
- Commit message: `Initial commit: FDP Gas Station Finder - Hybrid`
- Click "Commit changes"

### 4️⃣ You're Done with GitHub
- Your repo URL: `https://github.com/YOUR_USERNAME/rfro12-fdp-gas-station-finder`

---

## Vercel Deployment (1 click, 30 seconds)

### 1️⃣ Go to Vercel
- Visit: https://vercel.com

### 2️⃣ Sign In with GitHub
- Click "Sign up" (or "Continue with GitHub" if you have an account)
- Authorize Vercel to access GitHub

### 3️⃣ Import Your Repository
- Click "New Project" or "Import Project"
- Select your GitHub repo: `rfro12-fdp-gas-station-finder`
- Vercel auto-detects it's an HTML project
- Click "Deploy"

### 4️⃣ Wait ~30 seconds
- Vercel deploys your app
- You get a live URL

### 5️⃣ Your Live App
**URL format:** `https://rfro12-fdp-gas-station-finder.vercel.app`

(Vercel may customize the domain; you can also add your own)

---

## Testing Your Live App

1. **Open the URL** in your browser
2. **Upload sample-data.csv** (from the same GitHub repo)
3. **See the map load** with gas stations
4. **Test filters** (Province, Municipality, Status, Oil Company)
5. **Click markers** to view station details
6. **Export CSV** to verify it works

---

## Sharing with Your Team

Once live, share:
```
https://rfro12-fdp-gas-station-finder.vercel.app
```

Instructions for users:
1. Open the URL (no login, no download needed)
2. Drag-drop your CSV file or Excel
3. View the interactive map
4. Use filters, add/edit stations
5. Export data for backup

---

## If Something Goes Wrong

### "Repository not found"
→ Verify repo name: `rfro12-fdp-gas-station-finder`  
→ Make sure it's **Public** (not Private)

### "Blank page when deployed"
→ Check: Is the file renamed to `index.html`?  
→ If still blank: Check Vercel deployment logs (look for errors)

### "Map loads but data won't upload"
→ Verify CSV format matches specification  
→ Check file columns: Name, Address or Lat/Lng, Oil Company, Status

### "Can't sign into Vercel"
→ Use GitHub sign-up (create account if needed)  
→ Authorize Vercel to access your GitHub repos

---

## Long-term Maintenance

Once deployed:
- **Update the app?** Edit `index.html` on GitHub → Vercel auto-redeploys
- **Share with regions?** Give them the live URL (no download needed)
- **Backup data?** Export CSV from the app anytime

---

## Complete Timeline

| Step | Time | What to Do |
|------|------|-----------|
| 1. Create GitHub account | 2 min | https://github.com/signup |
| 2. Create repo & upload files | 3 min | https://github.com/new |
| 3. Go to Vercel | 30 sec | https://vercel.com |
| 4. Sign in with GitHub | 1 min | Authorize Vercel |
| 5. Import & deploy | 1 min | Click "Deploy" |
| 6. Wait for deployment | 30 sec | Watch progress |
| **TOTAL** | **~8 minutes** | **Your app is live!** |

---

## Your Live App is Now:
✅ Accessible from any browser  
✅ Works on desktop, tablet, mobile  
✅ No installation needed  
✅ Can be shared via URL  
✅ Auto-updates when you update code on GitHub  

---

**Status:** Ready for live deployment  
**Next:** Execute GitHub setup → Vercel deployment → Live!
