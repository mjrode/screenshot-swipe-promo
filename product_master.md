# Screenshot Swipe — Master Product Document

> **Status**: Work in Progress — Phase 1 (Core Feature Documentation)
> **Last Updated**: February 7, 2026

---

## The Problem

We all screenshot things we want to remember — delivery tracking, recipes, confirmation codes, shopping ideas, work notes, addresses. But screenshots pile up silently. Within days, we've forgotten *why* we took them. Our camera roll becomes a graveyard of good intentions.

**The core issue**: There is no built-in system on your phone to *act on* the things you capture. Screenshots are easy to take but impossible to organize, and the context behind them fades fast.

---

## The Core Message

> *What should someone understand about this app in 5 seconds?*

**Founder's intent**: "Use this app if you take screenshots of things you want to remember to do or look into but forget to review your screenshots and lose context on why you took them."

### Candidate Core Messages (Pick One)

| # | Message | Angle |
|---|---------|-------|
| **A** | **Never forget why you took a screenshot.** | Context preservation — emotional, resonant |
| **B** | **Your screenshots have a purpose. This app helps you act on it.** | Action-oriented — bridges capture → action |
| **C** | **A 2-minute daily habit that turns screenshots into action.** | Habit + speed — tangible promise |

> [!NOTE]
> **Recommendation**: Message **A** is the strongest for App Store first impression — it's short, emotional, and immediately understood. Message **C** works well as a supporting line (subtitle or second screenshot). Message **B** could be the promo page hero.

---

## What Screenshot Swipe Does

Screenshot Swipe turns your camera roll from a passive dumping ground into an **active system for keeping, organizing, and acting on** the things you capture.

It does this through a simple daily habit: **get reminded → review → decide → enrich → move on.**

---

## Target User

People who take a lot of screenshots and want to:
- Stop forgetting why they took them
- Keep their camera roll clean
- Turn captures into searchable, actionable information
- Build a simple daily habit around it (< 2 minutes/day)

**Secondary audience**: People who want to organize and annotate their *photos* as well (supported via the Screenshots/Photos toggle — wider appeal but not the primary positioning).

---

## App Name Assessment

> [!WARNING]
> **Current problem**: Searching "Screenshot Swipe" on the App Store does not surface the app. This is a critical discoverability issue.

**Issues with "Screenshot Swipe":**
- "Swipe" implies a simple gesture, but the app does much more (AI, profiles, batch processing)
- The name doesn't convey the *benefit* — it describes a mechanic
- ASO competition: "screenshot" is a crowded keyword

**Name alternatives to explore:**

| Name | Pros | Cons |
|------|------|------|
| **Captr** | Short, memorable, implies capture + action | Spelling could confuse |
| **ScreenNote** | Clear — screenshot + notes = the core value | A bit literal |
| **Recall** | Emotional — "remember why you took it" | Generic, may be taken |
| **Shotlog** | Screenshot + log = organized history | Not immediately clear |
| **Swipe & Save** | Describes the mechanic + the outcome | Still mechanic-focused |

> This is worth researching further — we should check App Store availability and keyword volume for top candidates.

---

## Core Workflow: The Daily Review

This is the heart of the app — a **daily triage habit** that takes under 2 minutes.

### Step 1: Set Your Reminder

Choose when you want to be reminded (Morning/Afternoon/Evening/Custom). Configure how far back the app looks (24h, 3 days, 1 week, 2 weeks).

> **Why this matters**: The reminder is what turns this from "another app" into a **habit**. Without it, screenshots just keep piling up.

### Step 2: Get Notified

Daily notification tells you exactly how many screenshots are waiting. Tap it → straight to your review queue.

### Step 3: Swipe Through Your Queue

Two review modes from the Home screen:
- **Swipe** (One by one) — Go through each screenshot sequentially. Swipe gesture or tap the Keep/Delete buttons.
- **Smart** (AI-powered, PRO) — AI analyzes a batch at once.

Each screenshot is shown full-screen with two actions:
- 🗑️ **Delete** — Adds to a deletion queue
- ✅ **Keep** — Save it and optionally enrich it

### Step 4: Enrich What You Keep

When you tap **Keep**, you can:
- **Add a Note** — type context manually, or tap **Analyze** for AI-generated notes
- **Add Tags** — choose existing or create new color-coded tags
- **Set a Reminder** — get notified later to revisit this screenshot
- **AI Analyze** — one tap to auto-generate notes, suggest tags, extract key info

### Step 5: Export (Optional)

Create a **Styled Card** — screenshot with notes and tags overlaid — that saves to Photos. Useful for sharing context with others *or* personal archival.

### After Review: Cleanup

Deleted items are **queued, not immediately removed**. At the end of a review session, the user is prompted to confirm bulk deletion from their phone — cleaning up storage without accidental loss.

> **Positioning note**: This is *not* a storage cleaner app. The cleanup is a natural byproduct of the review habit, not the primary value.

---

## Free vs. PRO Breakdown

| Feature | Free | PRO |
|---------|------|-----|
| Daily reminders & notifications | ✅ | ✅ |
| Swipe review (keep/delete) | ✅ | ✅ |
| Manual notes, tags, reminders | ✅ | ✅ |
| Explore view (browse, filter, search) | ✅ | ✅ |
| Styled card export | ✅ | ✅ |
| AI Analyze (single screenshot) | 3/day | Unlimited |
| Smart Review (batch AI analysis) | ❌ | ✅ |
| Smart Review Profiles | ❌ | ✅ |
| Deep Library Analysis (batch processing) | ❌ | ✅ |
| Auto-Analyze on Launch (auto-tag new screenshots) | ❌ | ✅ |

> [!NOTE]
> **Observation**: The free tier is generous — users get the full daily review workflow without paying. PRO unlocks AI automation and batch capabilities. This is a solid freemium model, but we should consider whether there's a friction point that makes free users *want* PRO (e.g., hitting the 3/day AI limit should feel like a natural upgrade moment, not a wall).

---

## Smart Review Profiles (PRO)

Smart Review Profiles let you teach the AI **how you want your screenshots organized**. Each profile is a reusable configuration that shapes how AI writes notes, what it pays attention to, and what it flags or deletes.

**When to use**: Any collection under ~100 images — your daily queue, a week's worth, or a month's screenshots.

### Profile Setup Wizard (4 Steps)

#### Step 1: Choose a Note Style

Controls the **tone and format** of AI-generated notes:

| Style | Description | Example Output |
|-------|-------------|----------------|
| **Casual & Brief** | Short, conversational — like texting a friend | *"Cool sneakers I want to buy"* |
| **Formal & Detailed** | Complete sentences with full context | *"Product listing for Nike Air Max 90, priced at $129.99 from Foot Locker"* |
| **Fun & Playful** | Witty descriptions with personality | *"Found my next flex — those kicks are fire 🔥"* |
| **Minimal (Tags Only)** | Skip notes entirely, just tags | *(no note — tags: #Shopping, #Shoes)* |
| **Actionable** | Focus on to-dos, action items, next steps | *"Order these shoes before the sale ends Feb 15"* |
| **Bullet Points** | Structured lists with key points | *"• Nike Air Max 90 • $129.99 • Foot Locker • Sale ends 2/15"* |
| **Technical** | Precise with technical details | *(detailed specs, code snippets, error messages)* |

#### Step 2: Select Focus Areas

Tells the AI **what topics to prioritize** when it encounters relevant screenshots. Screenshots matching these areas get richer, more detailed notes.

**Built-in categories**: Finance, Shopping, Recipes, Travel, Work, Personal, Tech, Health, Social Media

**Custom Instructions** (optional): Free-text to fine-tune AI behavior — e.g., *"For recipes, always list ingredients. For shopping, include prices and store names."*

> **How it works**: Focus areas don't *force* every screenshot into a category — they tell the AI "when you see something related to this, go deeper." A random meme still gets tagged as a meme.

#### Step 3: Flag Settings

Define keywords or tags that trigger **automatic flagging** in the review results. Flagged items get surfaced with extra visual attention so you don't miss them.

**Use case**: Flag anything containing "deadline", "receipt", "address", "confirmation code" — things you'd regret losing.

#### Step 4: Auto-Delete Rules

Pre-mark certain screenshots for deletion based on rules. **Safe & reversible** — items are pre-marked, not auto-deleted. You always confirm before anything is permanently removed.

Three rule types:
- **Delete by keywords** — If the AI note mentions these words (e.g., "receipt", "OTP", "verification")
- **Delete from apps** — Screenshots from specific apps (e.g., Twitter, Instagram, TikTok, Snapchat)
- **Delete by category** — Content types like Memes, Social Posts, Confirmations, OTP Codes, Ads

> **Marketing angle**: Auto-delete rules are powerful for users drowning in social media screenshots. "Stop manually deleting TikTok screenshots — let the AI handle it."

---

## Smart Review Workflow (PRO)

Batch AI analysis for collections under ~100 images — your daily queue, a week's backlog, or a monthly archive.

### Stage 1: Launch

From any collection on the Home screen (Yesterday, This Week, January 2026, etc.), tap the **Smart** button. Select the profile you want to use. If no profiles exist, the wizard launches first.

### Stage 2: Analysis

AI processes all images using the selected profile's settings (tone, focus areas, flag/delete rules). Progress shown live: *"Analyzed 10 of 18"* with the current screenshot visible.

### Stage 3: Results Grid

Once analysis completes, the **Results** screen shows a scrollable grid of all screenshots with:
- **Tags overlaid** on each thumbnail (e.g., #Tech, #Shopping, #Design)
- **AI-generated notes** visible in card format below each image
- A **"need attention"** banner at the top showing the count of flagged items with a "Review" button
- A **"Review One by One"** button at the bottom to enter sequential mode

**Tap-to-cycle**: Each grid card can be tapped to cycle between Keep (✅), Delete (🗑️), and Flag (🚩).

### Stage 4: One-by-One Review (Optional)

Tapping "Review One by One" enters a familiar view — the same full-screen Keep/Delete layout from the daily swipe review. The difference: **AI has already pre-filled the notes and tags**. User can:
- Review the AI-generated note (editable)
- See suggested tags (toggle on/off, add new)
- Set a reminder
- Accept or override the AI's Keep/Delete recommendation

### Stage 5: Confirmation

Tapping **Done** from the Results grid shows a summary dialog:
- ✅ *Marking X as reviewed*
- 🚩 *Flagging X for follow-up*
- 🗑️ *Deleting X screenshot(s)*

Confirm → all decisions are applied.

---

### ✅ Resolved: Flagging = Review Priority Only

**Decision**: Flagging is a **session-local** concept. Flag rules in profiles surface items to the top of the review queue during Smart Review (the "need attention" banner). After saving, items are simply **kept** or **deleted** — no persistent "flagged" status.

- The confirmation dialog simplifies to: **"Keeping X · Deleting X"**
- If a user wants persistent importance, they use **tags** or **reminders**
- Less concepts = less confusion

---

## Deep Library Analysis / Batch Processing (PRO)

A background AI job that can tag and annotate **thousands** of screenshots at once — ideal for onboarding new users who have months or years of backlog.

### How It Works

1. **Navigate to Deep Library Analysis** (Settings or Home)
2. **Choose scope**: Screenshots Only / All Photos
3. **Select a Smart Review Profile** — same profiles used in Smart Review (tone, focus areas, rules)
4. **Start Analysis** → Job runs in the background using a batch AI API
5. **Notification** when complete — results appear in Explore view

**Key capabilities** (shown in-app):
- **Smart Auto-Tagging** — AI analyzes every image and applies relevant tags (Recipe, Receipt, Memes, etc.)
- **Uses Your Profiles** — Applies focus areas, note style, and flagging rules from the selected profile
- **Archive & Organize** — Processed items are filed, keeping the main feed clean
- **Background Processing** — Runs silently; notification when done

### Queue Behavior Toggle

A **"Batch Removes from Queue"** setting (in Settings → Advanced) controls what happens after batch processing:

| Setting | Behavior | Best For |
|---------|----------|----------|
| **ON** | AI-tagged images are marked as reviewed and removed from the review queue | Users who trust the AI and want their queue cleared |
| **OFF** (default) | Images get notes + tags but **stay in the queue** for manual review one-by-one | Users who want AI to pre-populate but still want to swipe through each one |

> **Onboarding play**: New users can run a batch job on their entire library as the first thing they do — instant value. With the toggle OFF, they get pre-populated notes and tags as they swipe through the queue manually. With it ON, their backlog is instantly organized.

### Batch History

Each job shows:
- Profile used (e.g., "Tech/iOSapp")
- Date and time
- Status (Uploading, Processing, Complete)
- Option to **re-run** with a different profile

---

## Auto-Analyze on Launch (PRO)

Automatically tags and annotates **new screenshots** every time you open the app — no taps required. Your most recent screenshots are already enriched with notes and tags before you start reviewing.

### How It Works

1. **Open the app** → Auto-Analyze runs silently in the background
2. **Detects new screenshots** taken since the last analysis (up to 50 per session)
3. **Analyzes each screenshot** using your **default Smart Review Profile** — same tone, focus areas, and rules you've already configured
4. **Saves notes and tags** to each screenshot — pre-enriched and waiting in your review queue
5. **Progress banner** appears briefly: *"Auto-analyzing 12 of 50..."* → *"50 screenshots analyzed"*

### Key Details

| Setting | Value |
|---------|-------|
| **Cap** | 50 screenshots per session |
| **Profile used** | Your default Smart Review Profile |
| **Review status** | Screenshots are tagged but **not marked as reviewed** — they stay in your queue for manual confirmation |
| **Toggle** | Settings → AI Features → "Auto-Analyze New Screenshots" |
| **When it runs** | On every app launch and return from background |

> **Positioning note**: This is the "set it and forget it" companion to Smart Review. Smart Review is for intentional batch sessions. Auto-Analyze is the passive layer that keeps your queue pre-enriched so the daily review is faster — notes and tags are already there when you start swiping.

---

## Explore View

The library browser — a searchable, filterable grid of all your screenshots (or photos, via toggle).

### Layout

- **2-column grid** showing full screenshot cards with:
  - **Tags overlaid** in top-left corner (color-coded, e.g., #Shopping, #Tech, #Fitness)
  - **Status icons** at bottom of each card indicating: ✅ Reviewed, 🏷️ Tagged, 📝 Has Note, ⏰ Has Reminder
  - AI-generated notes visible in card body

### Filters

Three filter pills at the top:

| Filter | Options |
|--------|---------|
| **All** | Reviewed / Unreviewed |
| **Has** | Tag, Note, Reminder, Done (any combination) |
| **Tags** | Select specific tags — uses **additive (OR) filtering** so selecting multiple tags shows items matching *any* selected tag |

### Search

Pull down to reveal a search bar. Searches note content via text matching — find any screenshot by what the AI (or you) wrote about it.

### Detail View

Tap any card → full-screen detail view where you can edit notes, tags, and reminders. Same enrichment sheet used across the entire app.

---

## Streak Tracking & Gamification

Lightweight gamification that reinforces the daily review habit without being obnoxious.

### Celebrations

A floating capsule-style toast appears when you hit a milestone:

| Event | Trigger | Icon | Message |
|-------|---------|------|---------|
| **🔥 Day Streak** | Review on consecutive days | `flame.fill` | *"X Day Streak — Keep up the momentum"* |
| **⭐ Session Milestone** | Hit 5, 10, 25, 50, or 100 reviews in one session | `star.fill` | *"X In A Row! — You are on a roll"* |
| **✨ Cleanup Complete** | Clear a percentage of your library | `sparkles` | *"X% Cleaned — Library is looking better"* |

### How It Works

- **Streak**: Tracked per calendar day. Reviewing at least one screenshot extends the streak. Missing a day resets to 1.
- **Longest streak**: Persisted — users can see their personal best.
- **Session milestones**: Reset each session.
- **Auto-dismiss**: Celebrations appear for 3 seconds, then fade. Non-blocking (pass-through touch).

---

## Settings

Organized into logical groups:

| Section | Items |
|---------|-------|
| **Subscription** | Screenshot Swipe Pro status (Active), Manage Subscription, Restore Purchases |
| **Review** | Review Reminders (configure daily notification time), Stats & Insights (streak data, review counts), Find Duplicates |
| **Organization** | Manage Tags (create/edit/delete tags), Export Album (dedicated "Screenshot Swipe" album in Photos), Customize Collections (configure Home screen groupings) |
| **AI Features** (PRO) | Smart Review Profiles, Deep Library Analysis, Auto-Analyze New Screenshots (toggle) |
| **App** | Show Onboarding Guide, Restart Tutorial, App Permissions (→ system settings), Clear Batch Analysis (remove AI-generated notes & tags), Full Reset (⚠️ delete all tags, notes, reset app state) |
| **Advanced** | Batch Removes from Queue toggle (controls whether batch processing marks items as reviewed) |
| **About** | Version number (currently 2.4) |

---

## Marketing Strategy Notes

### The ORB Framework (from Launch Strategy research)

| Channel Type | Screenshot Swipe Assets | Status |
|-------------|------------------------|--------|
| **Owned** (you control) | Promo page, App Store listing, in-app onboarding | ✅ Active |
| **Rented** (algorithm-dependent) | App Store search, social media | ⚠️ ASO issues (name not discoverable) |
| **Borrowed** (others' audiences) | Influencer reviews, tech blogs, Reddit | ❌ Not started |

### Ongoing Launch Mindset
Every feature update is a re-launch opportunity. Recent updates (tutorial system, UI polish, Smart Review improvements) could each be marketed as moments to re-engage users.
