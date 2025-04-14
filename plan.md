Love that — let’s zoom out and make a **tactical battle plan** for how we’ll build this app from start to finish.

Here’s a **detailed phased game plan**, like a mini product roadmap, broken into small, bite-sized moves. We’ll focus first on local dev, then make it look nice, and later worry about hosting.

---

## 🧠 PHASE 1: Core Functionality Skeleton (Structure & Flow)

**Goal**: Just get the bones in place. Minimal styles. Focus on layout and navigation.

### ✅ 1. Routing (✅ done!)
- `/`: Dashboard page
- `/exercise/[id]`: Dynamic detailed view per exercise

### 🔜 2. Exercise Card Component
- Create `<ExerciseCard>` component
- Show name of exercise and dummy data (e.g. last weight/reps)
- Put a few sample cards on the dashboard
- Clicking a card → navigates to `/exercise/[id]`

### 🔜 3. Graph Component
- Create a `Graph.svelte` component using `svelte-chartjs`
- Use dummy data for now
- Show it in the exercise detail page

### 🔜 4. Workout Entry Table + Form
- Add a simple table of hardcoded entries (date, weight, reps, type)
- Add a form below the table to "add" a new entry (start with local JS, no DB)

---

## 🧱 PHASE 2: Data Layer Integration (DB & API)

**Goal**: Connect your frontend to real data via SvelteKit API routes and Prisma.

### 🔜 5. Setup Prisma API Routes
- Create API routes: `GET /api/workouts`, `POST /api/workouts`
- Use SQLite + Prisma to read/write actual data

### 🔜 6. Connect Frontend to API
- Fetch workouts for a specific exercise on detail page
- Display real workout data in the table and graph
- Submit new entries via the form

### 🔜 7. Week Grouping
- Use a helper function to calculate "week number" from workout dates
- Group workouts by week in the graph or display

---

## 🎨 PHASE 3: Design & Polish

**Goal**: Make it look professional using Tailwind + Figma designs (later).

### 🔜 8. Apply Tailwind Layout
- Use flex/grid for responsive layout
- Style the ExerciseCard nicely
- Add spacing, fonts, shadows, and icons from Lucide

### 🔜 9. Add Navigation Bar
- Add a top nav or side nav for future extensibility
- Consider mobile-responsiveness

---

## ☁️ PHASE 4: Hosting & Persistence (Future)

**Goal**: Make it public (optional)

### 🔜 10. Deploy
- Use Vercel (or Netlify) to host the frontend
- Persist your SQLite database or migrate to PostgreSQL (e.g. via Supabase, PlanetScale, or Neon)

---

## 🎯 Optional Cool Features (If You're Having Fun™)

- Toggle view: Hypertrophy vs Strength visual comparison
- Week-over-week line charts
- Form validation + success messages
- Animations (e.g., smooth card transitions)
- Dark mode (because why not)

---

## 🔥 Immediate Next Steps

We’re here in **Phase 1**. So let’s now:
> 🔨 Build the `ExerciseCard.svelte` component and render some cards on the dashboard with dummy data.

After that, we'll wire up clicking on cards to navigate to their detail pages.

Ready to build some exercise cards? 💪