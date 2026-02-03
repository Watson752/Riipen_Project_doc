# 🍽️ GTA Restaurant Directory – Web Development Plan  
**Website Developer Role | ATJ Consulting Inc.**

---

## 🎯 Overview

This project aims to build a **high-quality, user-friendly restaurant directory** for Toronto, designed to be scalable across the Greater Toronto Area. The platform will help restaurants improve visibility through listings and paid promotions, while providing users with an intuitive browsing experience.

The focus is to deliver a **clean, reliable MVP** that balances strong **UI/UX quality** with a tightly scoped feature set, ensuring maintainability and ease of future expansion.

---

## 🚀 Project Goals

- ✅ Deliver a **fully functional end-to-end directory**
- 🎨 Maintain **high UI/UX quality** with simple, intuitive flows
- 🛠️ Ensure the system is **easy to manage** for admins
- ⚙️ Use no-code tools efficiently without unnecessary complexity
- 📘 Leave the project in a **well-documented, handoff-ready state**

---

## 🧩 MVP Definition

### What MVP Means for This Project

For this project, MVP does **not** mean unfinished or low-quality.  
It means a **limited feature set executed well**, with polish, clarity, and reliability.

The MVP must clearly answer:
1. 🍴 Can restaurants be listed cleanly?
2. 🔍 Can users browse and filter listings easily?
3. 💳 Can restaurants pay to be promoted and see that reflected on the site?

If these are met, the MVP is successful.

---

### ✅ Included in MVP

- **Directory Pages**
  - `/city` – Browse restaurants by city with filters
  - `/now` – Highlight promoted listings and active offers
- **Owner Submission**
  - `/add` – Simple, trustworthy form for restaurant owners
- **Promotions**
  - `/promote` – Stripe checkout for paid promotion
  - Clear promotion rules and expiry
- **Database**
  - Businesses, Offers, and Recurring Rules (linked)
- **User Accounts (Lightweight)**
  - Email-based login for commenting only
  - Simple comments on listings (optional admin approval)
- **Initial Data**
  - Import and QA of first 100 restaurant records
- **Admin Experience**
  - Easy manual management and override where needed
- **Documentation**
  - One-page admin how-to and project walkthrough

---

### 🚫 Explicitly Out of Scope (for MVP)

- Full user profiles or social features
- Comment likes, replies, or feeds
- AI-driven recommendations or ranking
- Advanced analytics dashboards
- Custom mobile applications

These items are intentionally deferred to a future roadmap.
PS: If we include user accounts, I’d recommend limiting them to commenting only for MVP — simple login, simple comments, and optional admin approval. That keeps UX high and complexity manageable.

---

## 🎨 UX Principles & Quality Bar

High UI/UX quality is a priority. This will be achieved through **simplicity and consistency**, not feature overload.

### UX Principles
- 🧭 Clear, predictable navigation
- 🔁 Consistent layouts and reusable components
- ⚡ Minimal friction for core actions (browse, submit, promote, comment)
- ✍️ Clear copy and labeling
- 📱 Mobile-friendly by default

### UX Acceptance Criteria
- First-time users understand the site within seconds
- Filters respond quickly and behave predictably
- Forms feel short, clear, and trustworthy
- Promoted listings are visually distinguishable
- Commenting is simple and spam-resistant

---

## 🗃️ Data Model Overview

The system is designed **data-first**, ensuring all no-code tools stay aligned.

### Core Tables

**Businesses**
- Name
- Address
- City
- Cuisine (predefined options)
- Price range
- Status (Draft / Live)
- Promoted (true / false)

**Offers**
- Linked business
- Offer description
- Start date
- End date

**Recurring Rules**
- Promotion duration
- Renewal type (manual or recurring)

**Comments**
- Linked business
- Linked user
- Comment text
- Timestamp
- Status (Pending / Approved)

---

## 🔄 Automation Strategy

Automation improves efficiency but should not block reliability.

- ⚙️ **Preferred:** Automated promotion activation via Stripe webhook
- 🛑 **Fallback:** Manual admin toggle if automation requires iteration

Reliability and clarity take priority over complexity.

---

## ⏱️ 60-Hour Execution Plan

| Phase | Focus | Key Output |
|-----|-----|-----|
| Phase 1 (6–8h) | Scope & data model | Locked MVP + schema |
| Phase 2 (12–15h) | Core directory & UX | Working pages + filters |
| Phase 3 (10–12h) | Payments & promotions | Stripe checkout + logic |
| Phase 4 (12–15h) | Auth, comments, QA | Stable workflows + clean data |
| Phase 5 (8–10h) | Polish & handoff | Docs, admin guide, walkthrough |

The goal is to deliver a working MVP early and improve it iteratively.

---

## ⚠️ Risks & Mitigation

| Risk | Mitigation |
|---|---|
| Data inconsistency | Predefined tags + structured QA |
| Automation issues | Manual fallback option |
| Scope creep | Clear MVP boundaries + roadmap |
| UX churn | Early feedback and reusable patterns |
| Comment spam | Auth + optional admin approval |

---

## 🛣️ Future Roadmap (Post-MVP)

- Multi-city expansion across the GTA
- Enhanced analytics for restaurant owners
- Subscription automation improvements
- Advanced filtering and discovery features
- Richer community interactions (if validated)

---

## ✅ Final Note

This project prioritizes: **clarity, usability, and maintainability**.  
By keeping the scope focused and the UX polished, the directory will feel professional, reliable, and ready to scale beyond its initial launch.

