# StoryBrand Website Template System

Complete system for deploying conversion-focused websites for service businesses in under 30 minutes.

---

## WHAT THIS IS

A mobile-first website template with a single goal: get customers to send you a photo and their contact info. No forms to manage, no backend, no databases. Customer clicks button → uploads photo → fills basic info → their phone opens SMS app → they send it straight to your business number.

---

## FILES IN THIS REPO

### Core Template
- **index.html** - The actual website template (clone this for each client)

### Client Process
- **CLIENT_INTAKE_FORM.md** - Give this to clients to fill out
- **FORM_TO_PROMPT.md** - Shows you how to convert the form into an AI prompt
- **WORKFLOW.md** - Step-by-step instructions for applying generated copy

### Examples & Reference
- **CLIENT_PROMPT.md** - Blank AI prompt template (if you want to skip the form)
- **EXAMPLE_PROMPT.md** - Completed example showing what good input looks like

---

## WORKFLOW: NEW CLIENT SITE

### Step 1: Client Fills Form (15 min)
Send them `CLIENT_INTAKE_FORM.md`. They answer 18 questions about their business, problem, solution, services.

### Step 2: Generate Copy (5 min)
1. Use `FORM_TO_PROMPT.md` to convert their answers into AI prompt
2. Paste prompt into Claude
3. Claude generates 7 copy blocks ready to use

### Step 3: Apply Copy (5 min)
1. Clone `index.html`
2. Follow `WORKFLOW.md` to paste copy into 7 spots in the HTML
3. Save file

### Step 4: Rebrand (2 min)
1. Open `index.html` in browser
2. Press `Alt+A` to open admin panel
3. Upload client logo (colors extract automatically)
4. Enter client's phone number for SMS quotes
5. Done

### Step 5: Deploy (3 min)
Push to GitHub, deploy via GitHub Pages/Netlify/Vercel, or upload to client's hosting.

**Total time: ~30 minutes**

---

## HOW THE CONVERSION WORKS

1. Customer lands on site, sees their problem described
2. Clicks "Start Here" button
3. Form slides in: upload photo, describe problem, enter address + contact info
4. Clicks submit
5. Their phone's SMS app opens with everything pre-filled to your business number
6. They tap send
7. You get: photo, description, address, name, phone number

No backend. No database. No forms to manage. Pure conversion.

---

## CUSTOMIZATION

### What You Can Edit Without Breaking Anything:
- All text content in the HTML
- Logo (via admin panel)
- Colors (via admin panel or manual CSS)
- Service descriptions
- Number of services (add/remove service cards)

### What NOT to Touch:
- The form submission JavaScript
- The SMS link generation code
- The admin panel toggle (Alt+A)
- The ColorThief integration

---

## TECHNICAL DETAILS

**Stack:**
- Pure HTML/CSS/JS (no build process)
- Tailwind CSS via CDN
- ColorThief for logo color extraction
- Native `sms:` protocol for form submission

**Browser Support:**
- All modern mobile browsers (iOS Safari, Chrome, Firefox, Samsung Internet)
- Desktop browsers (for testing, but site is mobile-optimized)

**Hosting:**
- Static site - host anywhere
- GitHub Pages (free)
- Netlify (free)
- Vercel (free)
- Any standard web hosting

---

## TESTING CHECKLIST

Before delivering to client:

☐ Logo displays correctly  
☐ Colors look good (contrast, readability)  
☐ All text is client-specific (no template placeholders)  
☐ Phone number is correct in admin panel  
☐ Photo upload works on mobile  
☐ Form submission opens SMS app correctly  
☐ SMS message includes all customer data  
☐ Site is responsive (test on phone)  
☐ All links work  

---

## TROUBLESHOOTING

**Logo doesn't show after upload:**
- Check file size (keep under 2MB)
- Try JPG instead of PNG
- Clear browser cache

**Colors look wrong:**
- Logo might not have enough color contrast
- Manually set colors in admin panel CSS output
- Use color picker to adjust

**SMS doesn't open:**
- Only works on devices with SMS capability
- Desktop users won't see SMS app (expected)
- Test on actual phone, not emulator

**Form doesn't submit:**
- Check that phone number in admin panel has no formatting (just digits)
- Verify all form fields are filled
- Check browser console for errors

---

## FOLDER STRUCTURE FOR MULTIPLE CLIENTS

```
clients/
├── template/
│   └── index.html (master template)
├── client-abc-plumbing/
│   └── index.html (deployed version)
├── client-xyz-landscaping/
│   └── index.html (deployed version)
└── client-123-handyman/
    └── index.html (deployed version)
```

---

## LICENSE

Do whatever you want with this. No attribution required. It's a tool for your business.
