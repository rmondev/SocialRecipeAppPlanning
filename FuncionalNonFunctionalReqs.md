# 📘 Functional and Non-Functional Requirements Document
## Social Recipe App (Working Title)

---

## 🟢 1. Vision and Overview

A social platform for sharing and discovering home-cooked recipes with a vibrant community, featuring AI-powered tools to modify and enhance user-created recipes.

---

## 🟢 2. Target Users

- Home cooks
- Health-conscious individuals
- Beginner cooks

---

## 🟢 3. Unique Value Proposition

- Social-first experience with community following and engagement
- AI-powered recipe recommendations and modifications
- Rich recipe discovery and sharing capabilities

---

## 🟢 4. Functional Requirements

### 🔹 4.1 User Accounts & Authentication
- Users must be able to sign up and sign in with:
  - Google Single Sign-On
  - Apple Single Sign-On
- No email/password login or anonymous guest browsing.

---

### 🔹 4.2 User Profiles
- Each user profile includes:
  - Username
  - Profile photo/avatar
  - Bio/About Me
  - Location
  - Follower and following counts
  - Posted recipes
  - Personal cookbook (saved recipes)
- Profiles are **public by default**:
  - Users can mark individual recipes as **private** (visible only to themselves).
  - Users can set their cookbook to private.
- User roles:
  - Standard users
  - Admins/Moderators with abilities to delete content or suspend accounts
- Verified account badges are **planned for a future phase**, not included in MVP.

---

### 🔹 4.3 Recipe Creation
Users can create recipes with:
- Title
- Description
- Ingredients (list with quantities)
- Preparation steps
- Cooking time
- Difficulty level
- Cuisine/type tags (e.g., Italian, Vegan)
- General tags
- Nutrition information (potentially generated via AI)
- Cover photo (optional, can be auto-generated using AI)

---

### 🔹 4.4 Recipe Interaction
Users can:
- Like/favorite recipes
- Comment on recipes
- Reply to comments (nested replies)
- Like comments
- Rate recipes (star rating)
- Save recipes to their cookbook
- Share recipes externally (social media or direct link)

---

### 🔹 4.5 Recipe Discovery & Search
Users can:
- Search recipes by keyword
- Filter recipes by tags/cuisine
- Filter by difficulty and cooking time
- Browse trending recipes
- Receive AI-powered personalized recommendations
- View a feed of recipes from followed users

---

### 🔹 4.6 AI Features
Users can generate AI-powered recipe modifications, including:
- **Make Healthier**: Reduce calories or swap ingredients
- **Quick Version**: Reduce cooking time
- **Change Cuisine**: Adapt to another cuisine
- **Enhance Flavor**: Suggest improvements
- **Scale Recipe**: Adjust quantities for different servings

---

### 🔹 4.7 Social & Community Features
**Follows & Connections**
- Follow other users
- See who follows you
- Block other users

**Feeds**
- Personalized feed (followed users)
- Trending feed
- New Recipes feed
- Feeds are selectable via tabs
- Filter feeds by cuisine

**Notifications**
- Recipe liked
- Recipe commented on
- New follower
- Recipe featured
- Comment reply

**Reporting & Moderation**
- Report recipes and comments
- Block/report users
- Admin/moderator review tools

**Messaging**
- Messaging is **not included** in MVP

---

### 🔹 4.8 Recipe Privacy
- Users can mark recipes as private (visible only to themselves).

---

## 🟢 5. Non-Functional Requirements

### 🔹 5.1 Performance
- Recipe feed loads within **2 seconds** on average connections.
- AI-powered recipe suggestions return within **10 seconds**.
- Recipe uploads (including images) complete within **10 seconds**.

---

### 🔹 5.2 Scalability
- Designed for up to **1,000 users** initially.
- Firebase to handle auto-scaling beyond this if needed.

---

### 🔹 5.3 Availability & Reliability
- Standard availability target: ~**99% uptime**.

---

### 🔹 5.4 Security
- All connections encrypted via HTTPS.
- Tokens securely stored:
  - iOS: Keychain
  - Android: EncryptedSharedPreferences
- Firestore security rules:
  - Users can edit only their own recipes and profiles.
  - Private recipes visible only to their owner.
- Two-factor authentication is **not required**.

---

### 🔹 5.5 Privacy & Compliance
- Minimal privacy requirements for portfolio use.
- GDPR/CCPA and other compliance to be evaluated later if published.

---

### 🔹 5.6 Accessibility
- Accessibility support (screen readers, color contrast, text scaling) **planned for a later phase**.

---

### 🔹 5.7 Compatibility
- iOS minimum supported version: **iOS 13+**
- Android minimum supported version: **Android 8+**

---

## 🟢 6. Monetization (Future Phases)

Potential monetization options to be considered after MVP:
- In-app Ads
- Purchasable credits for premium AI features and recipe library
- Affiliate links for ingredients or tools
- Sponsored content (featured recipes)
- Donations via Patreon or in-app support

Timeline:
- Monetization is **not planned at launch** and will be evaluated in later phases if the app is published and gains adoption.

---
