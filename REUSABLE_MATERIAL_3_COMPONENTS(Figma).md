# 🧩 Reusable Material 3 Components (Figma)

This document outlines the reusable components to be designed in Figma using the Material 3 design system. These components will ensure visual consistency, speed up prototyping, and align with our React Native frontend implementation (e.g., React Native Paper).

---

## 🔘 Buttons

| Component        | Variants / Notes                              |
|------------------|-----------------------------------------------|
| Contained Button | Primary actions (e.g., "Publish", "Save")     |
| Outlined Button  | Secondary actions (e.g., "Cancel")            |
| Text Button      | Inline text actions (e.g., "Learn more")      |
| Icon Button      | Used for like, save, share, etc.              |
| FAB (Floating)   | For launching AI assistant (Feed only)        |

---

## ✏️ Inputs

| Component            | Use Cases / Variants                              |
|----------------------|---------------------------------------------------|
| Text Field           | Single-line for titles, usernames, etc.           |
| Multiline Text Field | For descriptions, bios, instructions              |
| Dropdown / Select    | Cuisine, Difficulty, Meal Type, etc.              |
| Radio Group          | Spice level, kid-friendly, gender, etc.           |
| Checkbox Group       | Ingredient exclusions, tags, dietary prefs        |
| Slider               | Portion quantity, calorie sliders (future)        |
| Switch / Toggle      | Privacy toggles (recipe, cookbook)                |

---

## 📇 Cards

| Component        | Description                                           |
|------------------|-------------------------------------------------------|
| Recipe Card       | Image, title, author, like/save/comment actions      |
| User Profile Card | Avatar, name, follow/unfollow button                 |
| Comment Card      | Nested replies, likes, timestamp                     |
| Notification Card | Used in notification feed                            |

---

## 📥 Modals / Overlays

| Component         | Use Cases                                            |
|-------------------|------------------------------------------------------|
| Confirmation Dialog | Save, delete, publish actions                      |
| Bottom Sheet       | Filter recipes, select tags                         |
| Full-Screen Dialog | AI recipe preview or enhancements                   |

---

## ⭐ Feedback UI

| Component          | Description                                         |
|--------------------|-----------------------------------------------------|
| Rating Star Picker | Rate recipes (1–5 stars)                            |
| Snackbar / Toast   | Quick feedback (e.g., "Recipe Saved")               |
| Progress Indicator | Loading AI results, uploads                         |
| Empty State Views  | No recipes found, empty cookbook, no connection     |

---

## 🧭 Navigation

| Component         | Notes                                                 |
|-------------------|--------------------------------------------------------|
| Tab Bar           | Feed, Cookbook, Create, Chefbot, Profile (5 tabs)     |
| Top App Bar       | Page title, back arrow, action icons                  |
| Search Bar        | With filter icon, used on Feed and Cookbook           |

---

## 👤 Avatar & Profile

| Component         | Notes                                                 |
|-------------------|--------------------------------------------------------|
| Avatar            | Circular, with fallback initial if no image           |
| Profile Header    | Cover image (optional), avatar, name, bio, stats      |

---

## 🔁 Component Guidelines

- **Variants:** Design each component with interactive states (default, hover, pressed, disabled).
- **Auto Layout:** Enable for responsiveness and consistency.
- **Text Styles:** Use Material 3 typography tokens (e.g., `bodyMedium`, `titleLarge`).
- **Color Tokens:** Use Material 3 color system (`primary`, `surfaceContainer`, `onPrimary`).
- **Elevation Levels:** Follow Material 3 elevation styles for cards, dialogs, FABs.

---

✅ These components will be stored in a shared Figma component library for consistent reuse across all screens.

