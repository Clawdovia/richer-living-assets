# Daily Build #008 Bonus — The 30-Minute Brand Site Checklist

**The exact sequence I used to go from "no site" to "live with SSL" in one afternoon.**

No page builder. No agency. No WordPress plugins. Just a stack that doesn't fight you.

---

## Stack (Free Tier Everything)

- **Framework:** Astro (static, fast, markdown-native)
- **Theme:** Dante (hero bio, dark mode, RSS, tags — built in)
- **Repo:** GitHub (Clawdovia org or personal)
- **Hosting:** Cloudflare Pages (300+ edge nodes, free, auto-deploys on push)
- **Domain:** Cloudflare Registrar (~$10/yr, no markup)

---

## The Checklist

### Phase 1 — Scaffold (10 min)
- [ ] Create GitHub repo: `yourusername/yoursite`
- [ ] Clone Astro + Dante starter: `npm create astro@latest`
- [ ] Edit `src/data/site-config.ts`: name, handle, tagline, Beehiiv subscribe URL
- [ ] Drop your headshot into `public/`
- [ ] Write your `src/pages/about.md` bio (be honest, not polished)

### Phase 2 — First Post (10 min)
- [ ] Create `src/content/blog/your-first-post.md`
- [ ] Add frontmatter: title, date, tags, excerpt
- [ ] Write something real — one thing you built, learned, or realized
- [ ] Commit and push to main

### Phase 3 — Deploy (5 min)
- [ ] Go to Cloudflare Pages → Connect GitHub repo
- [ ] Set build command: `npm run build`, output: `dist/`
- [ ] Deploy → live at `yoursite.pages.dev` in 60 seconds
- [ ] Add custom domain in Cloudflare Pages → DNS auto-configures
- [ ] SSL active within 2 minutes

### Phase 4 — Wire the Newsletter (5 min)
- [ ] Get Beehiiv subscribe URL from Grow → Subscribe Forms
- [ ] Paste into `site-config.ts` subscribe field
- [ ] Push → redeploy → subscribe form live

---

## Why This Stack

| Feature | Status |
|---------|--------|
| Zero attack surface | No database = nothing to hack |
| Zero hosting cost | Cloudflare Pages free tier is unlimited |
| Push-to-deploy | git push → live in 30 seconds |
| Training-data ready | Every post = structured markdown for future fine-tuning |
| RSS built-in | Readers can subscribe without giving you their email |

---

## The Real Lesson

You don't need a perfect brand to launch. You need a URL that's yours, a bio that's honest, and one post that's real.

Perfection is procrastination with a better excuse.

Ship the minimum. Iterate in public.

— Masa Wick
