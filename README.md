# Stree

**Your body. Your questions. Your space.**

Stree is a women's health companion. This repository holds the first front-end preview (MVP) so the idea can be shown and shared.

> **Preview only.** All answers, videos, myths and community posts are sample content for illustration. They are not clinically reviewed and are not medical advice.

## What is in the preview

| Tab | What it does |
| --- | --- |
| **Home** | Greeting, daily check-in, today's tip, a "For you" row that follows your life stage and interests, eight topic tiles, the "Nobody told me this" series, Myth vs Medicine, and "Ask without shame". |
| **Explore** | Search plus eight categories: periods, PCOS and hormones, sexual health, fertility, pregnancy, postpartum, menopause, and everyday wellness. 32 short sample video answers. |
| **Ask HerAI** | Type a question and get a short answer with its sources, when to get help, and related questions. Matches against the sample set only. |
| **Community** | Topic circles, anonymous posting, replies, "me too", save and report. |
| **My Profile** | Life stage, topics, language preference, privacy options, saved videos, watch history, and a way to view or delete your data. |

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
