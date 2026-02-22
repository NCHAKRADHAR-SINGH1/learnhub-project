# Study App Frontend

A modern React + Vite frontend for an educational platform, supporting student, teacher, and admin roles.

## Features

- User authentication (login/register)
- Role-based dashboards (Student, Teacher, Admin)
- Course browsing, enrollment, and payment
- Teacher course management (add/delete)
- Responsive UI with Bootstrap and Material UI
- API integration with backend (Express/MongoDB)

## Getting Started

### Prerequisites

- Node.js (v16+ recommended)
- npm

### Installation

1. Install dependencies:
	```
	npm install
	```

2. Start the development server:
	```
	npm run dev
	```

3. Open your browser at [http://localhost:5173](http://localhost:5173)

### Build for Production

```
npm run build
```

### Preview Production Build

```
npm run preview
```

## Project Structure

- `src/` - Main source code
  - `components/` - UI components for admin, user, common features
  - `assets/` - Images and static files
- `index.html` - Entry point
- `vite.config.js` - Vite configuration

## Environment Variables

Set your backend API URL in `.env`:
```
VITE_API_URL=http://localhost:8000
```

## Deployment

- Vercel configuration included (`vercel.json`)
- Output directory: `dist`

## License

MIT
