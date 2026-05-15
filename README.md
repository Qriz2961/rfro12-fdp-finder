# RFRO XII FDP Gas Station Finder

A non-technical web application for managing and locating participating gas stations in the LTFRB Fuel Discount Program (FDP) across Region XII.

## Features

- **File Upload** — Drag-and-drop CSV/Excel files with gas station data
- **Interactive Map** — Leaflet.js map with color-coded markers (green = participating, orange = issues, red = closed)
- **Smart Filters** — Province, Municipality, Status, Oil Company, Radius
- **Live Stats** — Real-time counts of stations by status
- **CRUD Operations** — Add, edit, delete, and modify station details
- **Data Export** — Export all data as CSV for audit trail
- **Local Storage** — Changes persist in browser

## Expected Data Format

Your CSV/Excel file should have these columns:

```
Name, Latitude, Longitude, Oil Company, Status, Station Code, Tarpaulin, DOE Remarks, Province, Municipality
```

### Status Values
- `participating` — Active in FDP program
- `issues` — Non-compliant (missing tarpaulin, incomplete paperwork, etc.)
- `closed` — Station not operational

### Tarpaulin Column
- `Y` or `1` = Posted
- `N` or `0` = Not posted

## Deployment to Vercel (1-Click)

### Step 1: Create GitHub Repository

1. **Go to GitHub** → https://github.com/new
2. **Repository name:** `rfro12-fdp-gas-station-finder`
3. **Public** (recommended)
4. **Create repository**

### Step 2: Upload Files

From your GitHub repo, upload:
- `index.html` (this is your entire app in one file)
- `README.md` (optional, for documentation)

Or clone locally and push:
```bash
git clone https://github.com/YOUR_USERNAME/rfro12-fdp-gas-station-finder.git
cd rfro12-fdp-gas-station-finder
# Copy index.html and README.md to this folder
git add .
git commit -m "Initial commit: FDP Gas Station Finder"
git push origin main
```

### Step 3: Deploy to Vercel

1. **Go to Vercel** → https://vercel.com
2. **Sign in with GitHub** (or create account)
3. **Import Project**
4. **Select your GitHub repo** → `rfro12-fdp-gas-station-finder`
5. **Deploy** (takes ~1 minute)

Vercel will give you a live URL like:
```
https://rfro12-fdp-gas-station-finder.vercel.app
```

## Usage

1. **Load the app** in your browser
2. **Upload your gas station data** (drag-and-drop CSV/Excel)
3. **Filter by Province, Municipality, Status, Oil Company**
4. **Click map markers** to see station details
5. **Edit or add stations** using the right panel
6. **Export data** as CSV anytime

## Data Persistence

- Changes are saved locally in your browser's storage
- To sync across devices, export and re-import the CSV
- For persistent backend storage, see Cloudflare Workers integration below

## Advanced: Cloudflare Workers Backend (Optional)

To add persistent cloud storage, contact your administrator with these requirements:

- Cloudflare Account
- D1 (SQLite) database
- Workers KV namespace
- Estimated setup: 2-3 hours

## Troubleshooting

**Maps not loading?**
- Check internet connection
- Clear browser cache (Ctrl+Shift+Delete)

**File won't parse?**
- Ensure Excel has columns: Name, Latitude, Longitude, Oil Company, Status
- Save as CSV if issues persist
- Check for special characters in cell values

**Filters not working?**
- Reload the page
- Re-upload your data
- Check that Province/Municipality fields are populated

## Support

For technical issues, contact your RFRO XII IT team or Chris Capistrano (Chief TDO).

---

**Version:** 1.0  
**Last Updated:** May 2026  
**Region:** RFRO XII (South Cotabato, Sultan Kudarat, Sarangani, General Santos City)
