# The Funders — Netlify CMS Setup

## What You Get

A complete content management system that lets you edit your entire website from a browser — no code needed.

## Admin Panel Sections

| Section | What You Can Edit |
|---------|-------------------|
| **Hero Section** | Headline, subtext, current rate, CTA buttons |
| **Niche Cards** | First-time buyers, newcomers, women & wealth content |
| **How It Works** | All 4 process steps |
| **Final CTA** | Headline, button text, link, guarantee text |
| **Footer** | Company description, NMLS ID, copyright |
| **Testimonials** | Add/edit client stories with star ratings |
| **Team Members** | Bios, photos, titles |
| **Blog Posts** | Full blog with markdown editor |
| **FAQ Items** | Questions & answers by category |
| **Glossary** | Mortgage terms & definitions |
| **Downloadable Guides** | PDF lead magnets |

## Setup Instructions

### Step 1: Create a GitHub Repo

1. Go to [github.com](https://github.com) and create a new repository called `thefunders-website`
2. Make it **public** (required for Netlify CMS free tier)

### Step 2: Upload These Files

Upload the entire contents of this folder to your repo:
```
thefunders-website/
├── admin/
│   ├── index.html
│   └── config.yml
├── content/
│   ├── hero.md
│   ├── niches.md
│   ├── process.md
│   ├── cta.md
│   ├── footer.md
│   ├── testimonials/
│   ├── team/
│   ├── blog/
│   ├── faq/
│   ├── glossary/
│   └── guides/
├── assets/
│   └── images/
└── index.html          ← Your main site file goes here
```

### Step 3: Connect to Netlify

1. Go to [netlify.com](https://netlify.com) → "Add new site" → "Import an existing project"
2. Select your GitHub repo `thefunders-website`
3. Deploy settings:
   - **Build command:** *(leave blank)*
   - **Publish directory:** `/` (or `.`)
4. Click **Deploy Site**

### Step 4: Enable Netlify Identity

1. In your Netlify dashboard → **Identity**
2. Click **Enable Identity**
3. Go to **Settings** → **Registration** → Set to **Invite only** (recommended for security)
4. Go to **Services** → **Git Gateway** → Click **Enable Git Gateway**
5. Invite yourself: **Identity** → **Invite users** → Enter your email

### Step 5: Access Your Admin Panel

1. Go to `https://your-site.netlify.app/admin/`
2. Click **Login with Netlify Identity**
3. Check your email for the invite link
4. Set your password
5. ✅ You're in! Start editing content

## How Editing Works

1. **Make changes** in the admin panel
2. **Save** — creates a draft
3. **Set status to "Ready"** — moves to review
4. **Publish** — triggers a new site deploy automatically

## Your Admin URL

After setup, bookmark this:
```
https://thefunders.ca/admin/
```

## Need Help?

- [Netlify CMS Docs](https://www.netlifycms.org/docs/)
- [Netlify Identity Docs](https://docs.netlify.com/visitor-access/identity/)
