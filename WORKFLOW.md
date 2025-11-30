# Client Intake Form - Complete Workflow Guide

## 🚀 Your End-to-End Process

### Step 1: Get the Form to Your Client

**Option A: Host it for free (Recommended)**
1. Go to [Netlify Drop](https://app.netlify.com/drop) or [Vercel](https://vercel.com)
2. Drag and drop `client-intake.html`
3. You'll get a URL like `https://your-intake-form.netlify.app`
4. Send this URL to every new client

**Option B: Send the file directly**
1. Email them the `client-intake.html` file
2. They open it in their browser
3. They fill it out and email/copy the results back to you

**Option C: Host on GitHub Pages (Free)**
1. Create a new repo on GitHub
2. Upload `client-intake.html`
3. Enable GitHub Pages in settings
4. Share the URL with clients

---

### Step 2: Client Fills Out the Form

Your client answers 6 simple questions:
- Business name
- What they do (1 sentence)
- 3 main services
- Phone number
- Logo (optional)
- Additional notes (optional)

**They see this at the end:**
- ✅ Success screen
- All their answers displayed
- **"Email These Answers"** button → Opens their email app with everything pre-filled
- **"Copy to Clipboard"** button → Copies all answers as formatted text

---

### Step 3: You Receive Their Answers

You'll get an email (or they'll paste) that looks like this:

```
CLIENT INTAKE FORM - NEW WEBSITE REQUEST
==========================================

Business Name: Joe's Landscaping

What They Do:
We handle tough landscaping jobs other companies won't touch - overgrown yards, steep slopes, and emergency cleanups.

Main Services:
1. Overgrown lot clearing
2. Difficult terrain work
3. Emergency storm cleanup

Phone: (555) 123-4567

Logo: ✓ Uploaded (see attachment)

Additional Info:
Green and brown colors preferred. Need it done by next week.

==========================================
Ready to generate copy and build the site!
```

---

### Step 4: Generate Copy with AI

**Copy the answers** and use the AI prompt template (see `AI-COPY-PROMPT.md`)

Paste their answers into the prompt and run it through ChatGPT, Claude, or any AI.

The AI will generate:
- Hero headline
- Hero subtext
- Problem section copy
- Solution section copy
- Service descriptions
- CTA text

---

### Step 5: Insert Copy into Template

1. Open your template site (`index.html`)
2. Find the sections marked with `id=""` attributes:
   - `id="heroHeadline"`
   - `id="heroSubtext"`
   - `id="problemText"`
   - `id="solutionText"`
   - `id="service1"`, `id="service2"`, `id="service3"`
   - `id="navBrand"`

3. Replace the placeholder text with AI-generated copy

4. Use the Admin Panel (press **Alt+A**):
   - Upload their logo
   - Colors automatically extract from logo
   - Copy CSS variables and save them

---

### Step 6: Customize Branding

**If they have a logo:**
1. Press `Alt+A` on the template site
2. Upload logo
3. Brand colors auto-extract
4. CSS is generated automatically

**If no logo:**
- Just use their business name (already in place)

---

### Step 7: Deliver the Site

1. Host their finished site (Netlify, Vercel, etc.)
2. Send them the URL
3. Collect payment 💰
4. Done!

---

## ⚡ Quick Reference

### Before You Send the Form:
- [ ] Change `YOUR_EMAIL_HERE` in `client-intake.html` line 534 to your actual email
- [ ] Host the form online (Netlify Drop is easiest)
- [ ] Bookmark the AI prompt template

### When You Get Responses:
- [ ] Copy their answers
- [ ] Paste into AI prompt template
- [ ] Generate copy
- [ ] Update template HTML
- [ ] Upload logo to admin panel
- [ ] Export and deliver

---

## 🎯 Pro Tips

1. **Save time:** Keep the AI prompt template open in a tab
2. **Batch process:** Collect multiple client intakes, then generate all copy at once
3. **Templates:** Save common variations (different industries) of generated copy
4. **Automation:** Use Zapier to auto-forward intake form emails to a dedicated folder
5. **Upsell:** Offer "premium customization" for clients who want more than the template

---

## 🔧 Customization

### To change your email in the form:
Edit line 534 in `client-intake.html`:
```javascript
const mailto = `mailto:your-email@example.com?subject=${subject}&body=${body}`;
```

### To add more questions:
- Copy a question group `<div class="question-group" data-question="X">`
- Update the question number
- Update `totalQuestions` variable in JavaScript
- Add the field to `formData` collection

### To change form styling:
- Edit CSS variables at the top of `client-intake.html`
- Change `--primary-color` and gradient colors

---

**That's it! You now have a repeatable system to onboard clients and build their sites fast.** 🚀
