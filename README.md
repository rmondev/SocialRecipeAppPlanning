# 🍳 Recipe Social Media App – Planning Repository

This repository contains all **project planning, documentation, and architecture** for the **Recipe Social Media App**, a social platform to share, discover, and enhance home-cooked recipes with the help of AI.

---

## 🎯 Overview

The Recipe Social Media App is designed as a **community-driven recipe platform** with:
- **Social-first experience** (feeds, following, likes, comments)
- **AI-powered tools** for recipe enhancements and generation
- A **rich recipe discovery** interface

This repository includes:
- Functional and Non-Functional Requirements
- Screen Flow Diagrams and User Journeys
- Data Models and Firestore Security Rules

---

## 📝 Documents

### 📘 Functional and Non-Functional Requirements
[FuncionalNonFunctionalReqs.docx](./FuncionalNonFunctionalReqs.docx)

Key highlights:
- **Authentication:** Google and Apple SSO only
- **Recipe Creation:** Manual editor and AI-powered modifications
- **Community Features:** Likes, comments, ratings, follows, notifications
- **Scalability:** Designed for up to 1,000 initial users
- **Performance Targets:** <2s feed loading, <10s AI recipe generation

---

### 📱 Screen Flows
[ScreenFlow.docx](./ScreenFlow.docx)

Includes complete flows for:
- **Onboarding and profile setup**
- **Bottom Tab Navigation:**
  - Feed (browsing and discovery)
  - Cookbook (saved recipes)
  - + (manual recipe creation)
  - Chefbot (AI exploration)
  - Profile
- **FAB:** A contextual floating button in the Feed for a **Guided AI Recipe Assistant**, with step-by-step MCQs:
  1. Meal Type
  2. Dietary Choices
  3. Regional Cuisine
  4. Kid Friendly
  5. Portion Quantity
  6. Portion Size
  7. Ingredient Exclusions
  8. Spice Level
- Manual creation and AI generation workflows
- Social interactions and error states

---

### 🛠️ Data Models & Firestore Design
[DataModelsAndSecurityRules.docx](./DataModelsAndSecurityRules.docx)

**Data Models Include:**
- **User Model:** Profiles with preferences and cookbook privacy
- **Saved Recipes:** Subcollection with notes and tags
- **Followers & Following:** Subcollections for social connections
- **Recipe Model:** Full recipe metadata including nutrition, tags, and visibility
- **Recipe Subcollections:**
  - Comments and likes
  - Ratings
  - Enhancements (AI-powered changes)

**Example Firestore Rules:**
- Users can edit only their own recipes and profiles
- Private recipes only visible to their owner
- Public recipes readable by all authenticated users
- Secure access to saved recipes respecting privacy flags

---

## 🧩 Technologies & Considerations

- **Firebase Firestore:** Real-time data storage
- **Firebase Authentication:** Google/Apple SSO
- **AI Integrations:** Recipe enhancements and generation
- **React Native:** Cross-platform app development
- **React Native Paper:** UI components (including FAB)
- **Accessibility:** Planned for later phases
- **Monetization:** Not included in MVP, but future options identified

---

## 🗺️ Next Steps

This planning repository will serve as the **source of truth** during development. Next milestones:
- Wireframes and high-fidelity mockups
- API contracts and OpenAPI documentation
- Detailed acceptance criteria and user stories
- Testing strategy and CI/CD setup

---

## ✨ Credits

Planning and documentation prepared for portfolio and potential production deployment.

---

## 📄 License

This project documentation is intended for educational and portfolio purposes. If you wish to use any materials commercially, please contact the author.
