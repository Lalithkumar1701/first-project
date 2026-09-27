# Pre-Deployment Verification Checklist

## Local Files Status (VERIFIED ✓)

### Main File
- [x] `index.html` exists (356 KB)
- [x] HTML file has correct `<img src="assets/...">` paths
- [x] No broken relative paths

### Assets Folder (18 Files)
- [x] `assets/about-community-care-large.jpg` (701 KB)
- [x] `assets/about-community-care.jpg` (84 KB)
- [x] `assets/about-hero-image.jpg` (628 KB)
- [x] `assets/asset-01.webp` (3.6 KB)
- [x] `assets/asset-02.webp` (114 KB)
- [x] `assets/asset-03.webp` (278 KB)
- [x] `assets/asset-04.webp` (189 KB)
- [x] `assets/asset-05.webp` (208 KB)
- [x] `assets/asset-06.webp` (163 KB)
- [x] `assets/asset-07.webp` (300 KB)
- [x] `assets/asset-08.webp` (432 KB)
- [x] `assets/asset-09.webp` (164 KB)
- [x] `assets/asset-10.webp` (133 KB)
- [x] `assets/asset-11.webp` (1,052 KB)
- [x] `assets/galvix-logo.png` (124 KB)
- [x] `assets/galvix-mark.png` (50 KB)
- [x] `assets/navira-hero.webp` (179 KB)
- [x] `assets/services-facilities-hero.webp` (48 KB)

### Configuration Files
- [x] `vercel.json` exists (1.13 KB)
- [x] `robots.txt` exists (0.08 KB)
- [x] `sitemap.xml` exists (1.33 KB)

### Code Quality
- [x] Spacing fixed: "Closer care, simpler visits. Comfortable spaces"
- [x] Zero "CLINIC HOURS" references
- [x] All image paths use `assets/` prefix
- [x] FormSubmit AJAX endpoint configured
- [x] Form uses `method="POST"` and correct action URL

---

## Deployment Steps

### Before You Deploy
- [ ] Close any file editors (optional, but recommended)
- [ ] Make sure you're logged into Vercel account
- [ ] Open File Explorer to: `c:\Users\vgana\OneDrive\Desktop\navira final\frontend\`

### During Deployment (METHOD 1 - Drag & Drop)

1. [ ] Go to https://vercel.com/dashboard
2. [ ] Click project: **navira-final-6**
3. [ ] Click **Deployments** tab
4. [ ] Select ALL files in `frontend/` folder:
   - [ ] `index.html`
   - [ ] `assets/` folder (entire folder)
   - [ ] `robots.txt`
   - [ ] `sitemap.xml`
   - [ ] `vercel.json`
5. [ ] Drag to Vercel deploy zone
6. [ ] Wait for deployment to complete (2-5 minutes)
7. [ ] Note deployment URL (e.g., "Preview: https://...")

---

## Post-Deployment Verification

### Immediate Checks (within 5 minutes)
- [ ] Vercel shows "✓ Production" status
- [ ] No deployment errors shown
- [ ] Latest deployment shows completed

### Browser Verification
- [ ] Visit: https://navira-final-6.vercel.app/
- [ ] Press **Ctrl+Shift+R** (hard refresh)
- [ ] Wait 10 seconds for images to load
- [ ] All images visible:
  - [ ] Navbar logo visible
  - [ ] Hero image visible
  - [ ] Doctor/staff photos visible
  - [ ] Clinic images visible
  - [ ] Service icons visible

### DevTools Verification (Press F12)

**Console Tab:**
- [ ] Zero `404` errors
- [ ] Zero `Failed to load resource` errors
- [ ] Zero `Uncaught` JavaScript errors

**Network Tab:**
- [ ] Filter by "Img" (images)
- [ ] All `.webp` files show **200** status
- [ ] All `.jpg` files show **200** status
- [ ] All `.png` files show **200** status
- [ ] No files show **404** status

**Application Tab (Optional):**
- [ ] Clear Site Data (optional, to clear cache)
- [ ] Refresh page

### Specific URL Tests

Open each URL in browser or DevTools (Network tab):

```
https://navira-final-6.vercel.app/assets/asset-01.webp
Expected: Image loads, HTTP 200

https://navira-final-6.vercel.app/assets/asset-02.webp
Expected: Image loads, HTTP 200

https://navira-final-6.vercel.app/assets/asset-03.webp
Expected: Image loads, HTTP 200

https://navira-final-6.vercel.app/assets/about-community-care-large.jpg
Expected: Image loads, HTTP 200

https://navira-final-6.vercel.app/robots.txt
Expected: Text file loads, HTTP 200

https://navira-final-6.vercel.app/sitemap.xml
Expected: XML file loads, HTTP 200
```

---

## Final Verification

- [ ] **All images loading** on https://navira-final-6.vercel.app/
- [ ] **Zero 404 errors** in DevTools Console
- [ ] **All asset URLs return 200** (verified in Network tab)
- [ ] **Spacing correct:** "Closer care, simpler visits. Comfortable spaces"
- [ ] **Zero clinic hours visible** anywhere on page
- [ ] **Form appears** in contact section
- [ ] **Responsive layout works** on mobile and desktop

---

## If Issues Remain

**Images still not showing?**

1. Check Vercel Dashboard → Deployments → Files tab
2. Verify `assets/` folder appears in Files list
3. If missing, redeploy using METHOD 2 (CLI) or METHOD 3 (GitHub)

**Getting 404s in DevTools?**

1. Hard refresh: **Ctrl+Shift+R**
2. Wait 30 seconds (CDN propagation)
3. Clear browser cache: **Ctrl+Shift+Delete**
4. Try incognito/private window

**Still broken?**

1. Contact Vercel support
2. Provide: https://navira-final-6.vercel.app/assets/asset-01.webp → 404

---

**Estimated Time:** 10-15 minutes total (deployment + verification)

**Current Status:** ✓ All local files verified. Ready to deploy.
