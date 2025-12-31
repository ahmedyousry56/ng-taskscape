# Taskscape - Frontend Application

> ITI Graduation Project - A modern Angular-based project management and task tracking application

Taskscape is a feature-rich frontend application built with Angular 16 that provides an intuitive interface for team members and scrum masters to manage projects, sprints, and tasks. It offers real-time updates, calendar views, and comprehensive task tracking capabilities.

## 🔗 Live Application

- **Frontend Application**: https://taskscape.vercel.app/
- **Admin Dashboard**: https://taskscape-admin.vercel.app/
- **Backend API**: Express Taskscape (see backend repository)

## ✨ Features

- **User Authentication**: Secure login system with JWT token management
- **Dashboard**: Personalized dashboard showing assigned projects and tasks
- **Project Management**: View and manage multiple projects with team members
- **Sprint Tracking**: Agile sprint management with timeline visualization
- **Task Management**: 
  - View assigned tasks with status, priority, and deadlines
  - Update task status (To Do, In Progress, Done)
  - Filter and sort tasks by various criteria
- **Calendar View**: Visual calendar representation of tasks and deadlines using Angular Calendar
- **Real-time Notifications**: Live updates via Socket.io for task changes and assignments
- **Responsive Design**: Mobile-friendly interface built with TailwindCSS and Angular Material
- **Role-based Access**: Different views and permissions for members and scrum masters

## 🛠️ Tech Stack

- **Framework**: Angular 16.2.0
- **UI Components**: 
  - Angular Material 16.2.11
  - PrimeNG 16.6.0
  - ngx-bootstrap 11.0.2
- **Styling**: 
  - TailwindCSS 3.3.3
  - Flowbite 1.8.1
  - FontAwesome 6.4.2
- **Calendar**: Angular Calendar 0.31.0 with date-fns
- **State Management**: RxJS 7.8.0
- **Real-time**: Socket.io Client 4.7.2
- **Notifications**: ngx-toastr 17.0.2
- **Authentication**: JWT Decode 4.0.0
- **Language**: TypeScript 5.1.3

## 📋 Prerequisites

- Node.js 16.x or higher
- npm or yarn package manager
- Angular CLI 16.2.2

## 🚀 Installation

1. **Clone the repository**:
   ```bash
   git clone https://github.com/yourusername/taskscape-frontend.git
   cd ng-taskscape
   ```

2. **Install dependencies**:
   ```bash
   npm install
   ```

3. **Configure environment**:
   Update the environment files in `src/environments/` with your backend API URL:
   ```typescript
   export const environment = {
     production: false,
     apiUrl: 'http://localhost:3000/api',
     socketUrl: 'http://localhost:3000'
   };
   ```

4. **Start the development server**:
   ```bash
   npm start
   # or
   ng serve
   ```
   Navigate to `http://localhost:4200/`. The application will automatically reload when you make changes.

5. **Build for production**:
   ```bash
   npm run build
   # or
   ng build
   ```
   Build artifacts will be stored in the `dist/` directory.

## 📖 Usage

### For Team Members

1. **Login**: Use credentials provided by your admin via email
2. **View Dashboard**: See all assigned projects and tasks at a glance
3. **Manage Tasks**: 
   - Click on tasks to view details
   - Update task status as you progress
   - View deadlines and priorities
4. **Calendar View**: Check upcoming deadlines and plan your work
5. **Notifications**: Receive real-time updates about new assignments

### For Scrum Masters

1. **Login**: Access with scrum master credentials
2. **Project Overview**: View all projects you're managing
3. **Sprint Management**: 
   - Create and manage sprints
   - Assign tasks to team members
   - Track sprint progress
4. **Task Assignment**: Create tasks with deadlines and priorities
5. **Team Monitoring**: Monitor team progress and task completion
6. **Notifications**: Get notified when team members update task status

## 🏗️ Project Structure

```
ng-taskscape/
├── src/
│   ├── app/
│   │   ├── components/      # Reusable UI components
│   │   ├── pages/           # Page components
│   │   ├── services/        # API and business logic services
│   │   ├── guards/          # Route guards
│   │   ├── interceptors/    # HTTP interceptors
│   │   ├── models/          # TypeScript interfaces and models
│   │   └── shared/          # Shared modules and utilities
│   ├── assets/              # Static assets (images, icons)
│   ├── environments/        # Environment configurations
│   └── styles.css           # Global styles
├── angular.json             # Angular CLI configuration
├── tailwind.config.js       # TailwindCSS configuration
└── package.json
```

## 🧪 Testing

Run unit tests:
```bash
npm test
# or
ng test
```

Tests are executed via [Karma](https://karma-runner.github.io) with Jasmine.

## 🎨 Development

### Generate Components
```bash
ng generate component component-name
```

### Generate Services
```bash
ng generate service service-name
```

### Generate Other Artifacts
```bash
ng generate directive|pipe|guard|interface|enum|module
```

## 🚀 Deployment

The application is deployed on Vercel. For manual deployment:

1. Build the production bundle:
   ```bash
   ng build --configuration production
   ```

2. Deploy the `dist/` directory to your hosting service

## 🤝 Contributing

This is an ITI graduation project. For contributions or suggestions, please contact the project team.

## 📝 License

This project is part of an educational program.

## 👥 Authors

ITI Final Project Team

## 📚 Further Help

For more information on Angular CLI:
- Run `ng help`
- Visit the [Angular CLI Documentation](https://angular.io/cli)
