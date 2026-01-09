# 📱 Jivo Care Flutter Assignment – Application Showcase

## Overview

This application was developed as part of a technical assignment to demonstrate **Flutter UI development, architecture design, and real-world app behavior**.

The focus of this project was not just visual accuracy, but **production-grade structure**, clean state management, offline handling, and thoughtful interaction design.

---

## 🎯 Goals of the Assignment

- Implement a complex, design-driven home screen
- Use modern Flutter best practices
- Demonstrate clean architecture and scalability
- Handle real-world scenarios like offline mode and lifecycle issues
- Deliver a polished, usable application

---

## 🧱 Architecture & Technical Approach

The app follows **Clean Architecture** principles with clear separation of concerns:

### Presentation Layer
- Flutter UI with **Bloc/Cubit** for state management
- Single immutable state per screen using `copyWith`
- Centralized async execution & error handling using a base Cubit guard
- Bottom navigation implemented using **Material 3 NavigationBar**
- `IndexedStack` used to preserve screen state across tabs

### Domain Layer
- UI-agnostic entities representing business data
- Use cases encapsulating individual actions
- Feature-level aggregation of use cases to keep Cubits clean

### Data Layer
- Separate **remote** and **local** data sources
- Remote layer uses Dio with a safe-call abstraction for consistent error handling
- Local layer simulates cached/offline data
- Centralized network-bound logic decides between remote and local sources

---

## 🌐 Offline & Network Handling

- Internet availability is handled centrally
- When offline, data is loaded from local sources
- When connectivity is restored, data refreshes automatically
- No connectivity or retry logic is duplicated across Cubits

---

## 🔍 Search & Interaction Highlights

- Dedicated search screen with auto-focus
- Debounced input handling to prevent unnecessary calls
- Safe lifecycle handling to avoid emit-after-close issues
- Smooth UI interactions (collapsing headers, carousels, expandable sections)

---

## 🎨 UI & UX

- UI implemented closely following the provided design
- Smooth animations for:
  - Collapsing header
  - Sticky search bar
  - Carousels and accordions
- Modern Material 3 components where applicable
- Focus on real app behavior rather than static screens

---

## ⚡ Development Approach (Vibe Coding – Used Responsibly)

To improve development speed, **vibe coding techniques** were used selectively —  
**but always in a controlled and reviewed manner**.

This means:
- AI assistance was used to accelerate boilerplate and iteration
- Architectural decisions, refactoring, and final implementations were **manually validated**
- No generated code was used blindly
- The final structure and logic reflect **intentional design decisions**

The goal was **efficiency without sacrificing quality or correctness**.

---

## 📦 Deliverables

### 📱 APK
👉 [**Download APK:**](https://github.com/rathorerahul586/JivoCare-demo-showcase/releases/download/v1/app-release.apk)


### 🎥 Screen Recording
👉 **Watch Demo Video:**  
https://drive.google.com/file/d/1059e-ZliVaWjA6LcDQ_8P1MnRtY1i7_V/view?usp=drive_link

The video demonstrates:
- App launch
- Key interactions
- Offline/online behavior
- Navigation and animations

---

## 🔒 Source Code Access

The complete source code is intentionally **not shared publicly**, as this assignment represents a significant body of work.

I’m happy to:
- Walk through the architecture
- Explain design decisions and trade-offs
- Discuss specific modules or patterns during a review or interview

---

## ✅ Summary

This project demonstrates:
- Production-grade Flutter architecture
- Clean and scalable state management
- Thoughtful handling of offline scenarios
- Strong attention to UX and interaction details
- A balanced approach between speed and quality

---

## 📩 Contact

If you have any questions or would like a walkthrough of any part of the implementation, I’d be happy to discuss it.

---

### ✨ Thank you for the opportunity to work on this assignment.
