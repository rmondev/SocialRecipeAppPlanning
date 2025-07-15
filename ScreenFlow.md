# 📱 Screen Flows – Recipe Social Media App

This document describes the primary screen flows for the Recipe Social Media App, including onboarding, profile setup, core navigation, manual recipe creation, guided AI recipe creation, social interactions, and cookbook browsing.

---

## 1️⃣ Onboarding & Authentication Flow

**Purpose:** Guide users through sign-in and initial setup.

**Screens:**
- Welcome Screen
  - App branding
  - “Continue with Google”
  - “Continue with Apple”
- SSO Authentication
  - OAuth flow via provider
- Profile Setup (First-Time Only)
  - Upload profile photo
  - Choose username
  - Optional: Bio and Location
- Onboarding Carousel (optional)
  - Short introduction slides explaining:
    - Feed for browsing
    - Create tab for posting recipes
    - FAB for AI-generated recipes
    - Cookbook for saved recipes
    - Profile and settings
- Landing on Feed tab

**Flow Summary:**
Welcome ➡️ SSO Authentication ➡️ Profile Setup ➡️ Onboarding Carousel ➡️ Feed Tab


---

## 2️⃣ First-Time Profile Edit Flow

**Purpose:** Allow new users to complete their profile right after onboarding.

**Screens:**
- My Profile (initial view)
  - Prompt to complete profile (banner or modal)
  - Edit Profile button
- Edit Profile
  - Update username, bio, location
  - Change profile photo
- Save changes

**Flow Summary:**
Profile Tab ➡️ Edit Profile ➡️ Save


---

## 3️⃣ Tab Bar Navigation Overview

After onboarding, users see the **bottom tab bar**, which is persistent across all screens:

**Tabs:**
1. Feed
   - Browse and discover recipes.
2. Cookbook
   - View saved recipes.
3. + (Create)
   - Manually create new recipes.
4. Chefbot
   - Explore AI tools and recommendations.
5. Profile
   - Manage profile and settings.

**Behavior:**
- Tapping **Create (+)** always opens the manual recipe editor.
- Tapping other tabs maintains navigation context.

---

## ✨ FAB Behavior

**Floating Action Button (FAB):**
- **Visible only on the Feed screen.**
- **Purpose:** Launch the Guided AI Recipe Assistant.
- **Behavior:**
  - Appears when scrolling up.
  - Hides when scrolling down.
  - Tapping starts a multi-step guided creation flow.

---

## 4️⃣ Home Feed & Discovery Flow (Feed Tab)

**Purpose:** Browse and discover recipes.

**Screens:**
- Home Feed
  - Tabs: Trending | Following | New
  - Filters: Cuisine, Cooking Time, Difficulty
  - Search bar
  - Recipe cards
  - **FAB:** "AI Recipe Assistant" (appears when scrolling up)
- Recipe Details
  - Title and description
  - Ingredients and instructions
  - Ratings and comments
  - Like, Save, Share
  - "Enhance with AI" button
- Search & Filters
  - Keyword search
  - Tag selection
  - Cuisine filter
- External Share
  - OS-native share sheet

**Flow Summary:**
Feed Tab ↔️ Recipe Details ↔️ Search/Filters ↔️ Share


---

## 5️⃣ Manual Recipe Creation Flow (+ Tab)

**Purpose:** Enable users to create and publish recipes manually.

**Access:** Tapping the + (Create) tab in the navigation bar.

**Screens:**
- Recipe Editor
  - Title and Description
  - Ingredients (add list)
  - Preparation steps
  - Cuisine and Tags
  - Difficulty, Cooking Time, Servings
  - Cover Photo (upload or AI-generated)
  - Nutrition Info (optional)
- Privacy Setting
  - Public / Private toggle
- Confirmation & Publish
- Return to Feed or Cookbook

**Flow Summary:**
Create Tab ➡️ Editor ➡️ Privacy ➡️ Publish


---

## 6️⃣ Guided AI Recipe Assistant Flow (Feed FAB)

**Purpose:** Help users generate a personalized AI recipe via guided questions.

**Access:** Tapping the FAB in the Feed screen.

**Screens:**

1. Meal Type
   - *Breakfast, Lunch, or Dinner?*

2. Dietary Choices
   - Vegan, Vegetarian, Keto, Paleo, No preference

3. Regional Cuisine
   - Italian, Mexican, Indian, Chinese, etc.

4. Kid Friendly
   - Yes / No

5. Portion Quantity
   - 1–10 servings

6. Portion Size
   - Small, Medium, Large

7. Ingredient Exclusions
   - Multi-select or free text input

8. Spice Level
   - Mild, Medium, Spicy

9. Confirmation
   - Review selections
   - "Generate Recipe" button

10. Generating Recipe
    - Loading animation

11. AI Recipe Preview
    - Title, Description
    - Ingredients and Instructions
    - Nutrition info
    - Optional image
    - Actions:
      - Save to Cookbook
      - Publish
      - Share externally

**Flow Summary:**
Feed FAB ➡️ Guided Questions (1–8) ➡️ Confirmation ➡️ Generate ➡️ Preview ➡️ Save


---

## 7️⃣ AI Exploration Flow (Chefbot Tab)

**Purpose:** Provide broader AI tools and recipe enhancement options.

**Screens:**
- Chefbot Home
  - Predefined AI suggestions
  - Recent enhancements
  - Quick actions:
    - Make Healthier
    - Quick Version
    - Change Cuisine
    - Enhance Flavor
    - Scale Recipe
- Enhancement Options
  - Select enhancement type
- Customization Parameters
- Generating Enhancement
- Enhanced Recipe Preview
  - Save to Cookbook
  - Share externally

**Flow Summary:**
Chefbot Tab ➡️ Enhancement Options ➡️ Customize ➡️ Generate ➡️ Preview ➡️ Save


---

## 8️⃣ Cookbook Flow (Cookbook Tab)

**Purpose:** View and manage saved recipes.

**Screens:**
- Cookbook Home
  - List of saved recipes
  - Filters (Tags, Cuisine)
  - Privacy toggle (Public/Private)
- Recipe Details (from saved list)
- Remove from Cookbook confirmation

**Flow Summary:**
Cookbook Tab ↔️ Recipe Details ↔️ Remove or Share


---

## 9️⃣ Social & Community Flow

**Purpose:** Support following, community engagement, and notifications.

**Screens:**
- User Profiles
  - Profile info
  - Follow / Unfollow
  - Followers / Following counts
  - Posted recipes
- Followers List
- Following List
- Notifications
  - Likes
  - Comments
  - Follows
  - Enhancements
- Report / Block Modal

**Flow Summary:**
Feed / Profile ↔️ User Profiles ↔️ Followers/Following ↔️ Notifications


---

## 🔟 Ratings & Comments Flow

**Purpose:** Enable recipe feedback and discussion.

**Screens:**
- Recipe Details
  - Ratings summary
  - Comments section
- Add Rating Modal
  - Star selection (1–5)
- Add Comment Modal
  - Text input
- Reply to Comment
  - Nested replies
- Like Comment
  - Inline action

**Flow Summary:**
Recipe Details ↔️ Add Rating ↔️ Comments ↔️ Replies


---

## 🔔 Error & Empty States

**Key Screens:**
- No Internet Connection
- Empty Feeds or Cookbook
- No Search Results
- Profile Incomplete
- Recipe Upload Failed

---

