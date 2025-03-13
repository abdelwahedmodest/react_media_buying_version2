# Django React Media Buying Project

This repository contains both the Django backend and React frontend for the Media Buying project. The project has been restructured to combine both components into a single repository for easier management and development.

## Repository Structure

```
django_react/
├── backend/         # Django backend code
└── frontend/        # React frontend code
```

## Setup Instructions

### Backend Setup

1. Navigate to the backend directory:
   ```bash
   cd backend
   ```

2. Create and activate a virtual environment:
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

4. Run migrations:
   ```bash
   python manage.py migrate
   ```

5. Start the Django development server:
   ```bash
   python manage.py runserver
   ```

The backend server will run at `http://127.0.0.1:8000/`.

### Frontend Setup

1. Navigate to the frontend directory:
   ```bash
   cd frontend
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Start the development server:
   ```bash
   npm run dev
   ```

The frontend development server will run at `http://localhost:5173/`.

## API Communication

The frontend is configured to communicate with the backend API at `http://127.0.0.1:8000/api`. If you need to change this configuration, update the `baseURL` in `frontend/src/services/api.js`.

## Development Workflow

1. Run both the backend and frontend servers simultaneously.
2. Make changes to the backend or frontend code as needed.
3. The frontend development server includes hot reloading, so changes will be reflected immediately.
4. For backend changes, you may need to restart the Django server depending on the nature of the changes.

## Original Repositories

This repository combines code from the following original repositories:
- Backend: [abdelwahedmodest/media_buying_django_react](https://github.com/abdelwahedmodest/media_buying_django_react)
- Frontend: [abdelwahedmodest/react_media_buying_version2](https://github.com/abdelwahedmodest/react_media_buying_version2)