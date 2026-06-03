# FlashTalks - Frontend

**FlashTalks** is a micro-talk marketplace where speakers publish 10–15 minute "flash" sessions. This repository contains the frontend client, focusing on delivering a fast, responsive, and accessible user experience for discovering and managing talks.

## Features

- **Event Discovery:** Fast, debounced search (300-400ms) with tag filters and paginated results.
- **Detail View:** Talk detail cards with a quick "Save" toggle for authenticated users.
- **Content Management:** Create and edit flash talk forms with robust client-side validation.
- **Authentication:** Google Sign-In integration. Displays user avatar/name when logged in and conditionally renders actions (e.g., hiding the create button for anonymous users).
- **Role-Based UI:**
  - **Regular Users:** Search, view, and save talks.
  - **Curators:** See admin controls to manage content (create, update, delete) ensuring quality and relevance.
- **Accessibility & Responsive Design:** Built with basic ARIA attributes and keyboard navigation support, fully responsive across devices.

## Tech Stack

- **Framework:** React / TypeScript / Vite
- **Styling:** Tailwind CSS (configured in `tailwind.config.js`)
- **Linting & Formatting:** ESLint + Prettier
- **Hosting:** Configured for Vercel deployment (`vercel.json`)

## Getting Started

### Prerequisites

- Node.js (v18+ recommended)
- npm or yarn

### Installation

1. Clone the repository and navigate to the frontend folder.
2. Install dependencies:
   ```bash
   npm install
   ```
3. Set up environment variables (copy `.env.example` to `.env` if available).
4. Run the development server:
   ```bash
   npm run dev
   ```

## Testing

Basic unit tests are configured to cover core functionalities such as Search and Pagination components. Run tests via:

```bash
npm test
```
