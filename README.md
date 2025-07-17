# 🍳 Recipe Social Media App – Planning Repository

This repository contains the **core planning documents**, screen flows, user journey definitions, data models, and wireframe checklists for the Recipe Social Media App—a social-first platform for discovering, sharing, and enhancing recipes using AI.

---

## 📌 Vision Statement

To create a vibrant and inclusive social platform where home cooks and food enthusiasts can share, discover, and enhance home-cooked recipes—powered by AI-driven personalization and community engagement.

---

## 👥 Target User Personas

1. **Home Cooks** – love cooking and sharing creations  
2. **Health-Conscious Individuals** – interested in nutrition and diet-specific modifications  
3. **Beginner Cooks** – need easy recipes and supportive tools

---

## 🌟 Unique Value Proposition

- **Social-first recipe sharing** with likes, comments, follows, and notifications  
- **AI-powered assistant** to help users create or enhance recipes through guided inputs  
- **Privacy-first controls** to keep recipes or cookbooks private  
- **Powerful discovery** through tags, filters, feeds, and AI personalization

---

## 📁 Included Documents

| File | Description |
|------|-------------|
| `FuncionalNonFunctionalReqs.docx` | Functional and Non-Functional Requirements |
| `ProjectVisionTargetUsers.docx`   | Vision, Personas, and Unique Value Proposition |
| `ScreenFlow.docx`                 | User Flows, Navigation, and Feature Screens |
| `DataModelsAndSecurityRules.docx`| Firestore Data Models and Security Rules |
| `ScreenChecklist.md`             | Wireframe screen checklist for development/design tracking |

---

## 🧭 Key App Flows

- **Onboarding & Authentication**  
- **Tab Bar Navigation** (Feed | Cookbook | + | Chefbot | Profile)  
- **Manual Recipe Creation** via the Create tab  
- **AI Recipe Assistant** accessed via FAB on the Feed  
- **Chefbot** AI exploration and enhancement tab  
- **Cookbook management**, saving, filtering, toggling privacy  
- **Community features**: profiles, followers, comments, likes, ratings  
- **Notifications & moderation**: alerts, reports, blocks  
- **Error & Empty States**

---

## ✅ Screen Checklist

View the full checklist in [`ScreenChecklist.md`](./ScreenChecklist.md)  
A preview:

- [ ] Welcome Screen  
- [ ] SSO Login (Google / Apple)  
- [ ] Profile Setup  
- [ ] Feed with FAB for AI assistant  
- [ ] Recipe Card & Detail View  
- [ ] Manual Creation Screens (+ tab)  
- [ ] AI Assistant Flow (multi-step MCQ)  
- [ ] Cookbook screens  
- [ ] Profile + Edit + Follower lists  
- [ ] Ratings, Comments, Notifications  
- [ ] Error and empty UI states

---

## 🔐 Firestore Data Models

See full details in [`DataModelsAndSecurityRules.docx`](./DataModelsAndSecurityRules.docx)

Includes:
- **User model** with preferences, saved recipes, followers/following
- **Recipe model** with ingredients, steps, images, tags, nutrition, enhancements
- **Subcollections** for:
  - Comments (with replies and likes)
  - Ratings (per user)
  - Likes (per user)
  - Enhancements (AI modifications)
- **Firestore security rules** for:
  - Profile data
  - Recipe visibility and ownership
  - Saved recipes (respecting privacy)

---

## 🧪 Functional Highlights

- Google/Apple SSO only (no password login)  
- Real-time feed and interactions  
- Manual and AI-enhanced recipe creation  
- Full CRUD with Firestore  
- Secure access control for public vs private content  
- MVP excludes messaging and monetization (planned for future)

---

## 🧱 Non-Functional Requirements (NFRs)

- Feed loads within **2 seconds**  
- AI responses within **10 seconds**  
- Supports **1,000 users initially**  
- 99% uptime expected  
- Minimum OS support: iOS 13+, Android 8+  
- Accessibility and monetization planned for later phases  

---

## 🛠 Tools and Technologies (Planned)

- React Native + Expo (frontend)  
- React Native Paper (UI components)  
- Firebase Firestore (database)  
- Firebase Auth (Google/Apple SSO)  
- OpenAI API for recipe generation & enhancement  
- GitHub Projects for tracking and collaboration

---

## 🗂 Milestones & Project Tracking

Project board is divided into 4 key planning milestones:

1. **Initial Planning Complete**
2. **Data Modeling & Security Design**
3. **Screen Flow & UX Design Complete**
4. **Final Review & Integration Prep**

Each milestone contains numbered issues with checklists and acceptance criteria.

---

## 📝 License

This project is created for educational and portfolio purposes only.

All documentation and materials are owned by the project author and may not be reused for commercial purposes without explicit permission. If you wish to reference, fork, or contribute, please contact the repository maintainer.

---

## 🤝 Contributing

At this stage, contributions are limited to planning and design collaboration. If you're interested in offering feedback or pairing on early development architecture, feel free to open an issue or submit a suggestion via the [GitHub Issues tab](../../issues).

---

## 🔗 Related Links

- [Project Board – Milestones & Issues](../../projects)  
- [Functional Requirements](./FuncionalNonFunctionalReqs.docx)  
- [Screen Flow](./ScreenFlow.docx)  
- [Data Models & Firestore Rules](./DataModelsAndSecurityRules.docx)  
- [Vision & Personas](./ProjectVisionTargetUsers.docx)  
- [Wireframe Screen Checklist](./ScreenChecklist.md)

---

## ✨ Author

**Riccardo Moncada**  
GitHub: [@rmondev](https://github.com/rmondev)  
LinkedIn: [linkedin.com/in/riccardomoncada](https://www.linkedin.com/in/rmondev)  

