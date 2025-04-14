## Overview
You’re building a web app for tracking workout progress where users interact with a dashboard composed of exercise cards. Each card provides quick insights into performance trends, while the detailed view includes interactive graphs, a comparison between hypertrophy and strength training, a historical data table, and a form to add new workout entries.

## Key Features
- Dashboard with Exercise Cards
- Each card represents a distinct exercise.
- Cards display summary metrics (e.g., latest weight/reps, recent progress trends).
- Interactive Graphs
- Integrate Chart.js through svelte-chartjs to visualize trends (such as the weight/reps ratio).
- Graphs update dynamically with new workout data.
- Detailed Exercise View
  - Clicking on an exercise card navigates to a detailed view.
#### The detailed page includes:
- A side-by-side comparison of hypertrophy vs. strength performance.
- A data table showcasing previous workout entries.
- A form for adding new workout records.
## Design and Styling
- Begin with a skeletal version; later incorporate a Figma design for a polished look.
- Use Tailwind CSS for responsive styling.
- Enhance user experience with Lucide icons.
## Local Database & API 
- Database: Use SQLite—a lightweight, file-based database ideal for local development.
- ORM: Use Prisma to define your data models and interact with the database seamlessly.
- API Endpoints: SvelteKit endpoints handle data fetching and updating (GET, POST, etc.) to interact with SQLite via Prisma.
## Technologies and Tools
- Frontend Framework: SvelteKit for reactive UI components and file-based routing.
- Styling: Tailwind CSS for quick, responsive styling.
- Icons: Lucide icons for modern, scalable iconography.
- Graphs: Chart.js (accessed via svelte-chartjs) for interactive data visualizations.
- Database & ORM: SQLite combined with Prisma for a lightweight yet scalable database solution.
- API Layer: SvelteKit endpoints (using +server.ts files) for managing data requests.
- Design Prototyping: Figma (in later stages) for detailed design and prototyping.