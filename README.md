# Organizo

Organizo is a web application for personal organization, focused on productivity, tasks, calendar, and daily motivation. The project was developed with React (Next.js), TypeScript, and TailwindCSS on the frontend, and Django with PostgreSQL on the backend, featuring a modern, responsive, and theme-customizable interface.

## Features

- **Task List:** Create, edit, complete, and organize tasks and subtasks.
- **Weekly Calendar:** View your week, see appointments and events with highlights for the current day and marked events.
- **Custom Themes:** Choose between themes like Classic, Sunset, and Ocean, each with unique visuals and colors.
- **Productivity Chart:** Track your performance over the last 7 days in a visual and interactive way.
- **Motivational Card:** Receive daily motivational quotes, with options to copy or change the phrase.
- **Accessibility:** Accessible interface, with keyboard navigation and theme-adjusted contrast.

## Technologies Used

- **Frontend:** React, Next.js, TypeScript
- **Styling:** TailwindCSS, CSS Modules
- **Icons:** Heroicons
- **Theme Management:** Context API
- **Backend:** Django (Python)
- **Database:** PostgreSQL

## Project Structure

```
organizo/
  ├── frontend/
  │   ├── src/
  │   │   ├── components/
  │   │   │   ├── CalendarWeek.tsx
  │   │   │   ├── ProductivityChart.tsx
  │   │   │   ├── MotivationalCard.tsx
  │   │   │   ├── Card.tsx
  │   │   │   ├── ThemeContext.tsx
  │   │   │   └── ...
  │   │   ├── pages/
  │   │   └── ...
  │   └── ...
  ├── backend/
  │   ├── organizo/
  │   ├── tasks/         # App for tasks and subtasks
  │   ├── users/         # App for user management and authentication
  │   └── core/          # Main app (project configuration, settings)
  └── ...
```

## Backend Overview

The backend is built with Django and provides a robust REST API for the frontend. The primary Django apps are:

- **tasks:** Handles creation, editing, completion, and organization of tasks and subtasks.
- **users:** Manages user registration, authentication (login/logout), and user profiles.
- **core:** Contains main project settings and primary configurations.

The database used is **PostgreSQL** for reliability, scalability, and advanced features.

## How to Run the Project

### Frontend

1. **Clone the repository:**
   ```bash
   git clone https://github.com/your-username/organizo.git
   cd organizo/frontend
   ```

2. **Install dependencies:**
   ```bash
   npm install
   ```

3. **Start the development server:**
   ```bash
   npm run dev
   ```

4. **Access at:**  
   [http://localhost:3000](http://localhost:3000)

### Backend

1. **Navigate to the backend folder:**
   ```bash
   cd ../backend
   ```

2. **Create and activate a virtual environment (optional but recommended):**
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. **Install the dependencies:**
   ```bash
   pip install -r requirements.txt
   ```

4. **Set up the PostgreSQL database and environment variables as needed.**

5. **Apply migrations:**
   ```bash
   python manage.py migrate
   ```

6. **Create a superuser (admin):**
   ```bash
   python manage.py createsuperuser
   ```

7. **Run the backend server:**
   ```bash
   python manage.py runserver
   ```

### API Usage

The backend exposes RESTful endpoints for tasks, users, and authentication. Detailed API documentation is available in the `/docs/` route if enabled or in the code comments.

## Theme Customization

- Access the theme settings in the app menu.
- Themes change not only the colors, but also the look of cards, buttons, and calendar elements.

## Contribution

Contributions are welcome!  
Open an issue or submit a pull request.

## License

This project is licensed under the MIT License.