# CV Builder

Приложение для создания резюме с современным дизайном и удобным интерфейсом.

## Разработка

```bash
# Установка зависимостей
npm install

# Запуск сервера разработки
npm run dev

# Сборка для production
npm run build
```

## Деплой

### Vercel (рекомендуется)

1. Установите Vercel CLI:
```bash
npm install -g vercel
```

2. Войдите в аккаунт Vercel:
```bash
vercel login
```

3. Деплой:
```bash
vercel
```

### Netlify

1. Установите Netlify CLI:
```bash
npm install -g netlify-cli
```

2. Деплой:
```bash
netlify deploy
```

### GitHub Pages

1. Добавьте в package.json:
```json
{
  "homepage": "https://yourusername.github.io/cv-builder",
  "scripts": {
    "predeploy": "npm run build",
    "deploy": "gh-pages -d dist"
  }
}
```

2. Установите gh-pages:
```bash
npm install --save-dev gh-pages
```

3. Деплой:
```bash
npm run deploy
```

## Структура проекта

- `src/` - исходный код
  - `components/` - React компоненты
  - `pages/` - страницы приложения
  - `contexts/` - React контексты
  - `types/` - TypeScript типы
  - `templates/` - шаблоны резюме
  - `styles/` - стили
  - `utils/` - утилиты
- `public/` - статические файлы
- `dist/` - собранное приложение

## Технологии

- React
- TypeScript
- Vite
- Material-UI
- React Router
- React Hook Form

## Features

- Intuitive form-based interface for entering CV data
- Multiple professional templates to choose from
- Real-time preview of your CV
- Export to PDF format
- Responsive design for all devices
- Local storage for saving progress

## Tech Stack

- React.js with TypeScript
- Material-UI for UI components
- react-hook-form for form handling
- @react-pdf/renderer for PDF generation
- React Router for navigation

## Getting Started

### Prerequisites

- Node.js (v14 or higher)
- npm or yarn

### Installation

1. Clone the repository:
```bash
git clone https://github.com/yourusername/cv-builder.git
cd cv-builder
```

2. Install dependencies:
```bash
npm install
```

3. Start the development server:
```bash
npm run dev
```

4. Open your browser and navigate to `http://localhost:5173`

## Project Structure

```
src/
  ├── components/
  │   └── editor/
  │       ├── PersonalInfo.tsx
  │       ├── WorkExperience.tsx
  │       ├── Education.tsx
  │       ├── Skills.tsx
  │       ├── Projects.tsx
  │       └── Languages.tsx
  ├── pages/
  │   ├── Home.tsx
  │   ├── Editor.tsx
  │   ├── Templates.tsx
  │   └── Preview.tsx
  ├── App.tsx
  └── main.tsx
```

## Usage

1. Start by selecting a template from the Templates page
2. Fill in your personal information, work experience, education, skills, projects, and languages
3. Preview your CV and make any necessary adjustments
4. Download your CV as a PDF

## Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

- Material-UI for the beautiful UI components
- react-pdf for the PDF generation capabilities
- All contributors who have helped improve this project 