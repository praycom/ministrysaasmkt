# America Prays — Partner Onboarding Workflow

## Overview

This document defines the recommended end-to-end workflow from the moment a ministry leader submits the form to become an America Prays Pray.com partner through full activation and ongoing engagement.

---

## Workflow Diagram

```
┌─────────────────────┐
│  STAGE 1: CAPTURE    │
│  Form Submission     │
└─────────┬───────────┘
          │
          ▼
┌─────────────────────┐
│  STAGE 2: QUALIFY    │
│  Internal Review     │
└─────────┬───────────┘
          │
     ┌────┴────┐
     │         │
  Approved   Declined
     │         │
     ▼         ▼
┌──────────┐ ┌──────────────┐
│ STAGE 3  │ │ Decline Email │
│ PROVISION│ │ + Alternative │
└────┬─────┘ └──────────────┘
     │
     ▼
┌─────────────────────┐
│  STAGE 4: ONBOARD    │
│  Welcome + Profile   │
└─────────┬───────────┘
          │
          ▼
┌─────────────────────┐
│  STAGE 5: ACTIVATE   │
│  Toolkit + Audience  │
└─────────┬───────────┘
          │
          ▼
┌─────────────────────┐
│  STAGE 6: ENGAGE     │
│  Events + Community  │
└─────────┬───────────┘
          │
          ▼
┌─────────────────────┐
│  STAGE 7: SUSTAIN    │
│  Ongoing Support     │
└─────────────────────┘
```

---

## Stage 1: Capture — Form Submission

**Trigger:** Ministry leader submits the Contact Us / Partner Interest form on AmericaPrays.com

**Form Fields Collected:**
- Full name
- Email address
- Organization name
- Organization type (church, ministry, nonprofit, media, other)
- Estimated audience/congregation size (optional)
- Message / reason for interest

**Immediate System Actions (Automated):**

| # | Action | System | Timing |
|---|--------|--------|--------|
| 1 | Store submission in CRM/database | CRM (e.g., HubSpot) | Instant |
| 2 | Tag contact as `partner-inquiry` | CRM | Instant |
| 3 | Send confirmation email to applicant | Email platform | Instant |
| 4 | Send internal notification to Partner Team | Slack / email alert | Instant |
| 5 | Create task in project management tool | Jira / Asana | Instant |

**Confirmation Email to Applicant:**
- Subject: "We received your America Prays partner request, [First Name]"
- Body: Thank them, set expectation for review timeline (48–72 hours), link to FAQ, provide partners@americaprays.com for questions
- This is NOT the welcome email — it's a receipt/acknowledgment only

---

## Stage 2: Qualify — Internal Review

**Owner:** America Prays Partner Team
**SLA:** Review within 48 hours of submission

**Review Checklist:**

| Check | Description | Pass/Fail |
|-------|-------------|-----------|
| Organization exists | Verify org has a website, social presence, or public presence | ☐ |
| Mission alignment | Organization is faith-based or prayer-aligned | ☐ |
| No brand conflicts | No messaging that conflicts with America Prays values (non-partisan, unity-focused, non-exclusionary) | ☐ |
| Contact is legitimate | Email is valid, person appears to represent the organization | ☐ |

**Qualification Outcomes:**

### Approved
- Update CRM tag to `partner-approved`
- Move to Stage 3: Provision
- Trigger approval notification

### Needs More Info
- Partner Team sends clarification email
- Applicant has 7 days to respond
- If no response → send one follow-up → close after 14 days

### Declined
- Update CRM tag to `partner-declined`
- Send decline email (gracious, non-specific)
- Suggest alternative ways to participate (join as an individual, attend events, share on social)
- Log reason internally for reporting

---

## Stage 3: Provision — Account & Page Setup

**Owner:** Pray.com Operations / Engineering
**SLA:** Within 24 hours of approval

**Actions:**

| # | Action | Owner | Details |
|---|--------|-------|---------|
| 1 | Create partner page URL | Engineering | e.g., `americaprays.com/[org-slug]` |
| 2 | Set up email capture on partner page | Engineering | Co-registration to Pray.com + America Prays |
| 3 | Enable prayer wall on partner page | Engineering | Linked to national prayer wall |
| 4 | Provision Partner Dashboard access | Engineering | Generate login credentials or magic link |
| 5 | Configure CSV tracking | Engineering | Attribute signups to this partner's page |
| 6 | Set up Prayer Widget embed code | Engineering | Pre-configured with partner's tracking ID |
| 7 | Update CRM tag to `partner-provisioned` | Ops | Trigger Stage 4 |

**Partner Page Includes:**
- Organization name and logo (placeholder until partner uploads)
- Email capture form (co-reg to Pray.com and the partner)
- Prayer wall
- Link to partner's website and social channels (once provided)
- America Prays branding

---

## Stage 4: Onboard — Welcome & Profile Completion

**Trigger:** Partner page and dashboard are provisioned
**Owner:** Automated email sequence + Partner Support Team

### Welcome Email (Day 0 — Sent immediately after provisioning)

- Subject: "You're in — welcome to America Prays, [First Name]"
- Content:
  - Confirm they're officially a partner
  - Share their unique partner page URL
  - Share Partner Dashboard login link
  - List what they need to complete their profile:
    - Logo (high-res PNG or SVG, transparent background)
    - Organization bio (150 words max)
    - Up to 3 prayer focus areas
    - Website & social media links
    - Primary contact name and email
  - CTA: "Complete Your Profile" → Dashboard link
  - Mention support contacts

### Profile Completion Reminder (Day 3 — Conditional)

- **Only sends if profile is incomplete**
- Subject: "[First Name], your partner page is almost ready"
- Dynamic checklist of missing items
- CTA: "Finish Your Profile"

### Profile Completion Confirmation (Triggered when profile is 100% complete)

- Subject: "[Organization Name] is live on America Prays!"
- Celebrate the milestone
- Show preview of their live partner page
- Transition to activation: "Now let's tell your community"

**Internal Tracking:**

| Metric | Target | Tracked In |
|--------|--------|------------|
| Profile completion rate | 80% within 7 days | CRM dashboard |
| Days to profile completion | < 5 days average | CRM dashboard |
| Support tickets during onboarding | Track volume & topics | Help desk |

---

## Stage 5: Activate — Toolkit & Audience Engagement

**Trigger:** Profile completed (or Day 7, whichever comes first)
**Owner:** Automated email sequence

### Toolkit Introduction Email (Day 7)

- Subject: "Your America Prays marketing toolkit is ready"
- Introduce assets available in the Partner Dashboard:
  - Social media kit (Instagram, Facebook, X templates)
  - Pre-written captions and hashtag guide (#AmericaPrays #Pray250)
  - Email templates (announcement, reminder series, recap)
  - Video assets (promo clips, b-roll, bumpers)
  - Logo package and co-brandable assets
  - Prayer Widget embed code for their website
- CTA: "Access Your Toolkit"

### Audience Activation Email (Day 14)

- Subject: "Time to tell your people, [First Name]"
- Challenge: Pick one channel, share once this week
- Three options:
  - **Email:** Use the announcement template
  - **Social:** Grab a graphic and post
  - **Stage:** Announce at next service with QR code
- CTA: "Download Your First Asset"

**Internal Tracking:**

| Metric | Target | Tracked In |
|--------|--------|------------|
| Toolkit access rate | 60% within 14 days | Dashboard analytics |
| First social post / email sent | 40% within 21 days | Self-reported or tracked |
| Widget embed rate | 20% within 30 days | Widget analytics |

---

## Stage 6: Engage — Events & Community

**Trigger:** Day 21+ post-onboarding
**Owner:** Automated emails + Partner Team

### Event Planning Email (Day 21)

- Subject: "Will [Organization Name] host a prayer event?"
- Four event ideas: Church Prayer Night, Community Gathering, Virtual Prayer Room, Small Group Prayer
- How to publish events on the national event map
- Key dates: June 28 (National Mall Rally), July 2–4 (Salute to America 250), July 4 (America Prays Day)
- CTA: "Create Your Event"

### Partner Spotlight & Community Email (Day 28)

- Subject: "See what other partners are doing"
- Movement stats (70+ partners, 1.2B combined reach)
- Feature a real partner story
- Monthly partner call invite (every 2nd Tuesday)
- Self-assessment checklist: profile, first post, event, team members
- CTA: "Register for the Next Partner Call"

### CSV Lead Delivery (Ongoing)

- **Frequency:** Weekly or bi-weekly (TBD based on volume)
- **Process:**
  1. System generates CSV of users who signed up on this partner's page
  2. CSV is attributed to the specific partner
  3. Email sent to partner's primary contact with CSV attachment
  4. Include summary: total new signups, cumulative signups, top referral sources
- **Format:** Name, Email, Date Signed Up, Page URL
- **Note from product spec:** The best delivery method still needs to be finalized — options include automated email, dashboard download, or API integration

---

## Stage 7: Sustain — Ongoing Support & Momentum

**Trigger:** Ongoing after Day 28
**Owner:** Partner Team + Automated campaigns

### Recurring Touchpoints

| Touchpoint | Cadence | Content |
|------------|---------|---------|
| Monthly Partner Newsletter | Monthly | Movement updates, new assets, partner spotlights, stats |
| Monthly Partner Call | 2nd Tuesday each month | Live updates, Q&A, peer connection |
| Milestone Countdown Emails | As dates approach | "60 days to go," "30 days," "1 week," "Tomorrow" |
| New Asset Alerts | As released | Notify when new graphics, videos, or templates are added |
| CSV Lead Reports | Weekly/bi-weekly | Signup data from their partner page |

### Countdown Activation Timeline

| Timeframe | Partner Actions | Pray.com Support |
|-----------|----------------|------------------|
| **Now – Spring 2026** | Complete profile, share first post, plan events | Onboarding emails, toolkit access, monthly calls |
| **May 2026 (60 days out)** | Switch to monthly social posts, send first email to list, finalize events | 60-day countdown email, activation timeline |
| **June 2026 (30 days out)** | Weekly social posts, send reminder email series, confirm events on map | Weekly check-in emails, promote National Mall Rally (June 28) |
| **June 29 – July 3** | Daily social posts, final reminder email, Sunday announcement | Daily push notifications, final activation checklist |
| **July 4, 2026** | Live coverage, host event, use #AmericaPrays #Pray250 | National coordination, real-time social amplification |
| **July 5–7, 2026** | Share recap content, thank community | Post-event recap email, impact stats, "what's next" |

### Re-Engagement for Inactive Partners

If a partner hasn't completed key milestones, trigger re-engagement:

| Condition | Action | Timing |
|-----------|--------|--------|
| Profile incomplete after 14 days | Personal email from Partner Team (not automated) | Day 14 |
| No toolkit access after 21 days | Phone call or personal email offering help | Day 21 |
| No social/email activation after 30 days | Partner manager outreach with simplified "just do one thing" ask | Day 30 |
| No activity after 45 days | Final outreach — "We're here when you're ready" + offer to simplify | Day 45 |
| No activity after 60 days | Mark as `partner-dormant` in CRM, stop automated sends, keep in monthly newsletter | Day 60 |

---

## Support Contacts for Partners

| Need | Contact |
|------|---------|
| General support | partners@americaprays.com |
| Marketing assets & co-branding | marketing@americaprays.com |
| Event planning & logistics | events@americaprays.com |
| Press & media inquiries | press@americaprays.com |
| General prayer inquiries | prayer@americaprays.com |
| Help Center | americaprays.com/partners/help |

---

## CRM Tags & Lifecycle Stages

Track each partner through the pipeline with these tags:

| Tag | Stage | Meaning |
|-----|-------|---------|
| `partner-inquiry` | Stage 1 | Form submitted, awaiting review |
| `partner-needs-info` | Stage 2 | Clarification requested |
| `partner-approved` | Stage 2 | Passed review |
| `partner-declined` | Stage 2 | Did not pass review |
| `partner-provisioned` | Stage 3 | Page and dashboard created |
| `partner-onboarding` | Stage 4 | Welcome sent, completing profile |
| `partner-profile-complete` | Stage 4 | Profile 100% done |
| `partner-activated` | Stage 5 | Has shared with audience at least once |
| `partner-event-planned` | Stage 6 | Has created or joined an event |
| `partner-fully-engaged` | Stage 6–7 | All key milestones hit |
| `partner-dormant` | Stage 7 | No activity after 60 days |

---

## Key Metrics Dashboard

| Metric | Description | Target |
|--------|-------------|--------|
| Form-to-approval rate | % of inquiries approved | 85%+ |
| Approval-to-provision time | Hours from approval to page live | < 24 hrs |
| Profile completion rate | % completing profile within 7 days | 80% |
| Toolkit access rate | % accessing dashboard assets within 14 days | 60% |
| Activation rate | % who share with audience within 30 days | 40% |
| Event creation rate | % who create or join an event | 30% |
| CSV delivery success | % of reports delivered on time | 100% |
| Partner call attendance | Average attendance per monthly call | Track trend |
| Partner NPS | Net promoter score from partner survey | 50+ |
| Dormant rate | % marked dormant after 60 days | < 20% |

---

## Open Items / Decisions Needed

These items from the product spec remain unresolved and need decisions:

| # | Item | Status | Owner |
|---|------|--------|-------|
| 1 | **CSV delivery method** — Automated email, dashboard download, or API? The spec notes "need to figure out the best way to send the emails to our America Prays partners" | Needs decision | Product + Engineering |
| 2 | **Partner page creation** — Manual by engineering or self-service through dashboard? | Needs decision | Product + Engineering |
| 3 | **Approval workflow** — Manual review or auto-approve with moderation? | Needs decision | Partner Team + Product |
| 4 | **Dashboard login** — Separate credentials, SSO via Pray.com, or magic link? | Needs decision | Engineering |
| 5 | **Prayer Widget metrics** — How are cross-site views aggregated and reported? | Needs decision | Engineering |
| 6 | **Email platform** — Which system sends the nurture sequence and CSVs? | Needs decision | Marketing + Engineering |
| 7 | **Co-registration flow** — How do signups on partner pages get attributed and shared with both Pray.com and the partner? | Needs decision | Product + Engineering |
