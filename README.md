# Fourwright — Website Kit

Everything the team needs to build and publish the Fourwright website.

```
fourwright-web-kit/
├── README.md              ← you are here
├── brand/
│   ├── BRAND_GUIDE.md     ← colors, fonts, logo rules, voice
│   └── logo/              ← all logo files (SVG + PNG)
└── site/                  ← the website, ready to publish
    ├── index.html         ← the page (text and structure)
    ├── styles.css         ← the design (colors, fonts, layout)
    └── assets/            ← logo and icons used by the page
```

The page is a single landing page: header, hero, services, the Databricks audit offer,
how we work, why us, team, contact and footer. It already works on phones.

## Step by step

### 1. Tools (once)
- GitHub account, **VS Code** and **Git** installed.
- VS Code extension **Live Server**.

### 2. Create the repo (Carlos)
1. On GitHub: **New repository** → name `fourwright-web` → Public → **Add a README**.
2. **Settings → Collaborators** → invite Miguel, Camilo and Jose.

### 3. Add the kit
1. Clone the repo in VS Code (**Clone Repository**).
2. Copy everything inside `site/` into the repo folder. Copy `brand/` too.
3. Right-click `index.html` → **Open with Live Server**. You should see the page.
4. **Commit** ("Add website kit") → **Push**.

### 4. Fill in the placeholders
Search in VS Code for `[` (Ctrl/Cmd + Shift + F). Replace every placeholder:

| Placeholder | What to put |
|---|---|
| `[PRICE]` | Audit price (ask Jose) |
| `[ROLE]` | Role of Carlos, Miguel and Camilo (ask Jose) |
| `[CALENDAR LINK]` | Booking link (e.g., Calendly or Google Calendar) |
| `[EMAIL]` | Contact email (e.g., hello@fourwright.com once the domain exists) |
| `[LINKEDIN URL]` | Company LinkedIn page |

### 5. Split the work
- **Carlos:** header, hero, services, audit.
- **Miguel:** how we work, why us, team, contact, footer.
- **Camilo:** check the page on phones, write down anything that looks wrong, test every link.
- Rules: always **Pull** before starting. Small **Commit** + **Push** when you finish something.
  Don't edit the same section at the same time.

### 6. Publish (free)
GitHub → **Settings → Pages → Branch: main → Save**.
In a few minutes it is live at `username.github.io/fourwright-web`.

### 7. Next (later)
1. Buy the domain `fourwright.com` (check Porkbun or Namecheap; it should cost the normal price, not "premium").
2. Connect it in **Settings → Pages → Custom domain**.
3. Create the email on that domain and replace `[EMAIL]`.
4. Use `brand/logo/png/fourwright-profile-1080.png` for LinkedIn and GitHub profiles.

## How to change things
- **Text:** edit `index.html`. Each section starts with a comment like `<!-- ========== HERO ========== -->`.
- **Colors and fonts:** edit only the top of `styles.css` (`:root`). Use the colors in `BRAND_GUIDE.md`.
- **Stuck?** Ask Claude: *"In this index.html, add a section X with the Fourwright brand colors"* and paste the result.

## Before going live — checklist
- [ ] No `[` placeholders left
- [ ] All buttons and links work
- [ ] Looks good on a phone
- [ ] Favicon shows in the browser tab
- [ ] Jose reviewed the text
