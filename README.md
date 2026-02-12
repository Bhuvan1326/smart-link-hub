# Smart Link Hub 

Smart Link Hub is a modern **Link-in-Bio / Link Hub Builder** that lets users create customizable hubs, manage links, apply smart rules, and track performance with analytics.

Build dynamic link pages that adapt based on **time, device, and custom conditions**, with click/visit tracking powered by Supabase.

---

## Features

- Authentication (Sign Up / Login)
- Create & manage multiple hubs
- Add / edit / enable-disable / delete links
- Public hub page using unique slug: `/u/:slug`
- Analytics:
  - Hub visits tracking
  - Link click tracking
- Rule Engine:
  - Time-based rules
  - Device-based rules
  - Performance-based rules
- Dark theme with neon green accents
- Built with shadcn/ui components & TailwindCSS

---

## Tech Stack

- **Frontend:** React + TypeScript + Vite
- **UI:** Tailwind CSS, shadcn/ui, Lucide-react Icons
- **Backend:** Supabase (DB + Auth)
- **Deployment:** Vercel

##  Live Deployment
- **Vercel App:** https://smart-link-hub-nine.vercel.app
- **Public Hub Example:** https://smart-link-2zzdrka2l-bhuvan-patils-projects-2aca3b63.vercel.app/dashboard/hubs/806826b4-91ce-4165-b86e-fdfa837fd129

## 📂 Project Structure
```txt
src/
├─ components/
│  ├─ ui/
│  ├─ DashboardLayout.tsx
│  ├─ LinkEditor.tsx
│  ├─ NavLink.tsx
│  ├─ ProtectedRoute.tsx
│  ├─ RuleBuilder.tsx
│  └─ SortableLinkItem.tsx
│
├─ hooks/
│  ├─ use-mobile.tsx
│  ├─ use-toast.ts
│  ├─ useAnalytics.ts
│  ├─ useHubs.ts
│  ├─ useLinks.ts
│  └─ useRules.ts
│
├─ integrations/
│  └─ supabase/
│     ├─ client.ts
│     └─ types.ts
│
├─ lib/
│  ├─ auth.tsx
│  ├─ rule-engine.ts
│  ├─ types.ts
│  └─ utils.ts
│
├─ pages/
│  ├─ auth/
│  │  ├─ Login.tsx
│  │  └─ Signup.tsx
│  │
│  ├─ dashboard/
│  │  ├─ Analytics.tsx
│  │  ├─ Dashboard.tsx
│  │  ├─ HubDetail.tsx
│  │  └─ NewHub.tsx
│  │
│  ├─ Index.tsx
│  ├─ NotFound.tsx
│  └─ PublicHub.tsx
│
├─ test/
│  ├─ example.test.ts
│  └─ setup.ts
│
├─ App.css
├─ App.tsx
├─ index.css
├─ main.tsx
└─ vite-env.d.ts
│
supabase/
├─ migrations/
└─ config.toml
│
vercel.json
.env
.gitignore
package.json
vite.config.ts
