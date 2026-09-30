# PlayCash Prelander — Deploy Guide

This repo is a static, single-page prelander. No build step is needed.

## Files at the repository root

```
playcash/
├── index.html    # the entire prelander (device check → qualify → rewards → offer CTA)
├── vercel.json   # Vercel hosting settings (picked up automatically)
└── DEPLOY.md     # this guide
```

## Deploy with Vercel

1. Go to [vercel.com](https://vercel.com) and sign in with GitHub.
2. Click **Add New… → Project**.
3. Under **Import Git Repository**, find `leeshanamud-droid/playcash` and click **Import**.
4. In the project setup screen:
   - **Framework Preset:** Other (or None)
   - **Root Directory:** `./` (default)
   - **Build Command / Output Directory:** leave blank
5. Click **Deploy**.

Vercel builds in seconds and gives you a live URL like `playcash-xxxx.vercel.app`.

## Notes

- The CTA button points to the affiliate offer with TikTok macros
  (`__CAMPAIGN_NAME__`, `__AID_NAME__`, `__CID_NAME__`) left untouched — TikTok
  replaces them with real values when the ad runs.
- To update the page later, edit `index.html` and commit; Vercel redeploys automatically.
