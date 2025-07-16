# 🧾 Dev Handoff & Design Audit — Week 1 UI/UX Sprint

## ✅ Summary

This document serves as the developer handoff package for the Week 1 UI/UX sprint. It includes Figma links, component specs, interaction notes, and all necessary resources to begin frontend development using a ShadCN/Tailwind-aligned system.

---

## 🎨 Component Kit

### Base Components

| Component | States                                    | Notes                                   |
| --------- | ----------------------------------------- | --------------------------------------- |
| Button    | `default`, `hover`, `disabled`, `loading` | Includes icon support and size variants |
| Input     | `empty`, `filled`, `error`, `disabled`    | Supports helper text + validation       |
| Modal     | `open`, `closing`, `scrollable`           | Escape key and click-outside support    |
| Card      | `default`, `elevated`, `selected`         | Used in project/task views              |
| Avatar    | `default`, `with status`, `fallback`      | Circle variant with fallback initials   |

🔗 **Figma Link**: [Component Kit](https://www.figma.com/file/...)

---

## 🖥️ Key Screens

### Responsive Mockups

| Screen        | Desktop | Mobile | Notes                                  |
| ------------- | ------- | ------ | -------------------------------------- |
| Auth          | ✅       | ✅      | Includes error states, password toggle |
| Dashboard     | ✅       | ✅      | Uses Auto Layout, responsive grid      |
| Project View  | ✅       | ✅      | Kanban layout with drag-and-drop       |
| Task Modal    | ✅       | ✅      | Focus trap + editable rich text        |
| Team Settings | ✅       | ✅      | Role management, invite flow           |
| Chat (opt-in) | ✅       | ✅      | Emoji picker, markdown preview         |

🔗 **Figma Link**: [Screen Mockups](https://www.figma.com/file/...)

---

## 🔄 User Journeys

| Flow                 | Tool Used | Notes                               |
| -------------------- | --------- | ----------------------------------- |
| Auth & Session Flow  | Figma     | Gated screens + reset password      |
| Task Lifecycle       | Miro      | Create → Assign → Update → Complete |
| Team Management      | Miro      | Invite → Accept → Role change/leave |
| Error/Empty Handling | Notion    | Defined for each screen interaction |

📌 Edge cases documented in **Notion: [UX States](https://www.notion.so/...)**

---

## 📐 Specs & Constraints

* **Spacing**: 4pt baseline grid, spacing tokens via Figma Variables
* **Typography**: Tailwind `font-sans`, heading/body sizes mapped
* **Radius**: 8px for cards, 4px for buttons/inputs
* **Colours**: Derived from Tailwind theme, light + dark variants
* **Motion**: `ease-in-out`, 150ms transitions (hover, modal, dropdown)

---

## 🔧 Dev-Ready Exports

* Figma Dev Mode enabled on all components
* Component layer names follow `PascalCase` matching codebase
* Variants structured using Figma’s `Component Properties`

📁 **Assets**: Exported icons, illustrations, and SVGs stored in `assets/ui-kit/`

---

## 📚 References

* [Component Mapping Sheet](https://docs.google.com/spreadsheets/d/...) — Figma ↔ ShadCN primitives
* [Design Archive](https://github.com/...) — Screenshots, decision logs
* [UI Guidelines](https://www.notion.so/...) — Brand tokens, tone, spacing rules

---

## 🧪 Audit Checklist

* [x] All base components support all interaction states
* [x] Mobile + desktop breakpoints tested
* [x] Dark mode previewed
* [x] Figma file structured with `Pages` and naming conventions
* [x] Comments added for conditional logic / implementation notes
* [x] All flows prototyped + linked

