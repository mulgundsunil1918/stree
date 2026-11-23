# Stree

**Your body. Your questions. Your space.**

Stree is a women's health companion. This repository holds a clickable front-end preview so the idea can be shown, shared and tested with real people.

> **Preview only.** Every answer, video, doctor, lab, price, post and number is sample content for illustration. None of it is clinically reviewed and none of it is medical advice. Nothing is booked, ordered, sent or charged.

Live preview: https://mulgundsunil1918.github.io/stree/

## What is in the preview

Five tabs, with sub-sections inside Explore and My Profile.

| Tab | What it does |
| --- | --- |
| **Home** | Greeting, today card (cycle day, check-in, tip), a featured video, quick tools, topic tiles, "Nobody told me this", Myth vs Medicine, a care teaser, the FAQ, and "Ask in private". |
| **Explore** | **Videos** (search, 8 topics, 32 short sample video answers), **Tools**, **Know your body**, **Myths**, **Care**. |
| **Ask HerAI** | Ask in the open and get a short answer with sources and when to get help. Or **Ask without shame**: a private question that goes to the staff queue. Voice input where the browser supports it. |
| **Community** | Topic circles, anonymous posting, replies, reactions, save, report, block, and a safety check on every post. |
| **My Profile** | Account, life stage, conditions, date of birth, consent choices, language, saved videos, and delete-my-data. Sub-sections: **Journey**, **Reminders**, **My care**. |

### Explore

- **Tools**: period and ovulation calculator, due date and pregnancy week, BMI and healthy range, pelvic floor timer, wellness challenges (7 and 14 day), and a lab report explainer for 9 common tests.
- **Know your body**: tappable reproductive anatomy, a day-by-day hormone chart with phase notes, and a week-by-week pregnancy slider.
- **Myths**: Myth vs Medicine cards with category filters and search.
- **Care**: doctors (book, reschedule, cancel), labs (cart and home collection), pharmacy (prescription request), nutrition programmes, and webinars and events. Sample providers and prices.

### My Profile

- **Journey**: daily check-ins, a private health timeline, a 14-day trend view, a doctor summary you choose what goes into, and CSV export.
- **Reminders**: pills, appointments and period reminders. Browser notifications if you allow them, plus a discreet mode that hides the wording.
- **My care**: your appointments, lab orders, prescription requests, programmes and event registrations.

### Safety and privacy

- **Teen safeguards** when the date of birth is under 18: posting is forced anonymous, the BMI tool is replaced by a message, pharmacy is blocked, and booking carries a trusted-adult note.
- **Community screening** blocks links, contact details, adverts and dose advice. Posts that suggest self-harm open a support sheet (Tele-MANAS 14416 for India, findahelpline.com elsewhere) and, if shared anyway, are flagged urgent for moderators.
- **Consent choices** for AI, research and notifications, and a one-tap way to erase everything stored on the device.

### Languages

English, Kannada, Hindi, Telugu, Tamil and Malayalam. The menus, tabs and headings switch language. The medical content stays in English until it can be translated and reviewed by clinicians who speak the language.

### Staff preview

Open it from the "Staff preview" link in the footer (`#admin`). There is no real sign-in: you pick a role (administrator, medical reviewer, moderator or content creator) and see only what that role would see.

- **Content**: draft, send for review, approve or request changes, with a version history. Approved videos and FAQ items appear in the app.
- **Review queue**: a reviewer checklist that must be completed before approving.
- **Categories**: add or remove topics and see them appear on Home and Explore.
- **Moderation**: reports from the community, with remove and restore.
- **Questions**: answer the private questions asked on the same device through "Ask without shame".
- **AI sources**: turn trusted sources on or off for the content editor.
- **Users** and **Dashboard**: sample data only.

## What is real and what is sample

| Works for real, on this device | Sample or simulated |
| --- | --- |
| All calculators, the timer, the lab explainer (rule-based), the cycle and pregnancy views | Doctors, labs, pharmacy, programmes, events and every price |
| Check-ins, timeline, doctor summary, CSV export | Videos: an illustrated presenter with live captions and optional read-aloud |
| Reminders and notifications while the page is open | "AI" answers: matched against the sample set by keywords |
| Teen safeguards, post screening, report, block, remove | Sign-in: demo only, the code is `123456` |
| Staff content workflow, categories, FAQ and ask queue (shared between the two views on this device) | Dashboard numbers, users and reports from other people |
| Language switching for menus and headings | Medical content in other languages |

Preferences, check-ins, posts, reminders and staff data are kept in the browser's local storage only. Nothing is sent to a server.

## Built for phones

Tab bar at the bottom, 44px touch targets, 16px inputs (no zoom on iOS), edge-to-edge scrolling rows, bottom-sheet dialogs and video player, and safe-area support for notched phones.

Deep links work: `#tools-cycle`, `#tools-due`, `#tools-bmi`, `#tools-pelvic`, `#tools-challenge`, `#care-labs`, `#journey`, `#reminders`, `#mycare`, and `#video-<id>` to open a video.

## Run it

No build step. Open `index.html` in a browser.

```bash
open index.html
```

## Structure

Everything lives in one file, `index.html`:

- `<style>`: design tokens at the top of the stylesheet, then components.
- `<script>`: content data, then state and storage, translations, views, routing, the player, the sheets, the staff preview, and event handling.

## Not built yet

This is a front-end preview, so the following need real work before launch:

- A backend and database, with real accounts, sign-in and one-time codes.
- A real AI service that retrieves from verified sources, with clinical review of every answer.
- Real video production and an authoring pipeline.
- Real booking, lab, pharmacy and payment integrations, with the legal and licensing they need.
- Clinician-reviewed translations of the medical content.
- Server-side moderation, audit logs and role-based access for staff.
- Accessibility and security audits, and a privacy review for health data.
