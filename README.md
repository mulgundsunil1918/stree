# Stree

**Your body. Your questions. Your space.**

Stree is a women's health companion. This repository holds the first front-end preview (MVP) so the idea can be shown and shared.

> **Preview only.** All answers, videos, myths and community posts are sample content for illustration. They are not clinically reviewed and are not medical advice.

## What is in the preview

| Tab | What it does |
| --- | --- |
| **Home** | Greeting, daily check-in, today's tip, a "For you" row that follows your life stage and interests, eight topic tiles, the "Nobody told me this" series, Myth vs Medicine, and "Ask without shame". |
| **Explore** | Two sections. **Videos**: search plus eight categories (periods, PCOS and hormones, sexual health, fertility, pregnancy, postpartum, menopause, everyday wellness) with 32 short sample video answers. **Tools**: see below. |
| **Ask HerAI** | Type a question and get a short answer with its sources, when to get help, and related questions. Matches against the sample set only. |
| **Community** | Topic circles, anonymous posting, replies, "me too", save and report. |
| **My Profile** | Life stage, topics, language preference, privacy options, saved videos, watch history, and a way to view or delete your data. |

## Tools (Explore > Tools)

All tools work on this device only, with no sign-up. Results are estimates for information, not medical advice.

- **Period & ovulation calculator**: next period, ovulation and fertile window, a tap-to-set calendar, and a period log that works out your average cycle length.
- **Due date & pregnancy week**: from last period or conception date, with week, trimester and key dates.
- **BMI & healthy range**: metric or imperial, with WHO or South Asian ranges and the limits of BMI explained.
- **Pelvic floor timer**: guided squeeze and relax sets with adjustable hold and repeats.
- **Wellness challenges**: gentle 7 and 14 day habits with no targets or penalties.

Each tool has its own address, for example `#tools-cycle`, `#tools-due`, `#tools-bmi`, `#tools-pelvic` and `#tools-challenge`.

## Built for phones

Tab bar at the bottom, 44px touch targets, 16px inputs (no zoom on iOS), edge-to-edge scrolling rows, a bottom-sheet video player, and safe-area support for notched phones.

## Videos

The videos are placeholders: an illustrated presenter with live captions, played from the sample scripts. Nothing is sent to a server. Preferences, check-ins and your own posts are kept in the browser's local storage only.

## Run it

No build step. Open `index.html` in a browser.

```bash
open index.html
```

## Structure

Everything lives in one file, `index.html`:

- `<style>`: design tokens at the top of the stylesheet, then components.
- `<script>`: content data (categories, videos, myths, tips, sample posts), then state and storage, components, views, routing, the video player, and event handling.

## Not built yet

Sign-in and accounts, a real AI backend with source retrieval, real AI-presenter video, translations (the language choice is saved but content is English only), the cycle tracker, the moderator and admin panels, and doctor booking. The full product plan is in the master prompt this preview was built from.
