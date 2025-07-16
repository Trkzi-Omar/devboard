## 🔹 WEEK 2 FRONTEND FOUNDATION — DevBoard

### 🎯 Goal

Establish a production-grade frontend foundation using Next.js App Router with ShadCN UI components, TailwindCSS theming, and Zustand-based state scaffolding. Ensure the app layout, routing, and core layout primitives are developer-ready.

---

## 📅 Daily Breakdown

### **Day 1: Project Bootstrapping**

**Objective**: Scaffold the project structure and configure baseline tooling.

| Task                                         | Tool / Tech                 | Output                              |
|----------------------------------------------|------------------------------|-------------------------------------|
| Initialize Next.js App Router project        | create-next-app, TypeScript | Project skeleton                    |
| Install TailwindCSS + ShadCN + Lucide Icons  | Tailwind, ShadCN CLI         | Configured UI stack                 |
| Set up ESLint + Prettier + Husky             | ESLint, Prettier, Git Hooks | Code quality enforcement            |
| Create shared `lib`, `components`, `hooks`   | Project folder structure     | Scalable architecture               |

---

### **Day 2: App Shell & Layouts**

**Objective**: Build the global layout and responsive container structure using ShadCN primitives.

| Task                                  | Tool / Tech         | Output                       |
|---------------------------------------|----------------------|------------------------------|
| Build responsive sidebar/navigation   | Tailwind, ShadCN     | Sidebar, header, container   |
| Implement App Shell layout            | Next.js Layouts      | `/app/(dashboard)/layout.tsx` |
| Add mobile support via drawer menu    | ShadCN Drawer        | Mobile-friendly nav UI       |
| Apply theme tokens from Figma         | Tailwind config      | Consistent branding           |

---

### **Day 3–4: Routing & Page Templates**

**Objective**: Set up dynamic routes and stub core pages using Next.js App Router.

| Route                    | Purpose                                      |
|--------------------------|----------------------------------------------|
| `/dashboard`             | Projects overview                            |
| `/project/[id]`          | Project Kanban + details                     |
| `/auth/login`, `/signup`| Authentication flows                         |
| `/settings`              | User/team settings                           |
| `/`                      | Marketing/Landing (optional)                 |

| Task                                      | Tool / Tech      | Output                       |
|-------------------------------------------|------------------|------------------------------|
| Define layouts and nested routes          | App Router       | Page hierarchy               |
| Add metadata with `generateMetadata()`    | Next.js SEO      | SEO + dynamic titles         |
| Set loading and error UI states           | React Suspense   | UX during async fetches      |

---

### **Day 5: UI Primitives & Theming**

**Objective**: Set up reusable UI components and extend ShadCN theme defaults.

| Task                                 | Tool / Tech        | Output                         |
|--------------------------------------|---------------------|--------------------------------|
| Add custom Button, Input, Modal      | ShadCN CLI, Tailwind | Themed and accessible UI       |
| Style components to match Figma      | Tailwind tokens     | Visual fidelity                |
| Add dark mode support                | Tailwind config     | Theme toggle                   |
| Set up utility components (Loader)   | Reusable components | Shared feedback elements       |

---

### **Day 6: State Management Bootstrapping**

**Objective**: Prepare for interactive flows with client-side state scaffolding.

| Task                                 | Tool / Tech         | Output                           |
|--------------------------------------|----------------------|----------------------------------|
| Install and configure Zustand        | Zustand              | Global UI state store            |
| Create store slices (e.g. sidebar)   | Zustand patterns      | Modular state management         |
| Add persistence for auth/token       | Zustand + localStorage | Session memory (stubbed)         |

---

### **Day 7: Integration Testing & Polish**

**Objective**: Validate foundational frontend flows and prep for backend/API work.

| Task                                      | Tool / Tech        | Output                         |
|-------------------------------------------|---------------------|--------------------------------|
| Add Vitest + Testing Library setup        | Vitest              | Frontend test config           |
| Write smoke tests for layout/pages        | Vitest + JSDOM      | Working page tests             |
| Lint & format entire codebase             | ESLint, Prettier    | Clean codebase                 |
| Final review of routing and themes        | Manual check        | Ready for API integration      |

---

## 📦 Deliverables by End of Week 2

* 📁 Next.js project bootstrapped (App Router, TypeScript, ShadCN)
* 🧱 App Shell layout with responsive sidebar + drawer
* 🗂️ Routing setup with working page templates
* 🎨 Themed UI components (buttons, inputs, modals)
* 🌙 Dark mode toggle with persistent user preference
* 🧠 Zustand global state slices scaffolded
* ✅ Linting, formatting, and smoke test coverage
