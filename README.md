# Valentine's Day Special 💖

A fun and interactive Valentine's Day web app that asks someone to be your Valentine in the most adorable way possible. The "Yes" button grows larger with each "No" click, while the "No" button shrinks and evades your cursor!

## 🎯 Features

- **Interactive UI**: Fun animations and interactive buttons that respond to user input
- **Escalating Questions**: 30 different Valentine's prompts that get progressively more persuasive
- **Smart Button Behavior**:
  - "Yes" button grows exponentially with each "No" click
  - "No" button shrinks, moves around, and eventually disappears
- **Name Personalization**: Asks for the user's name before starting
- **Email Notifications**: Sends email notifications via EmailJS when someone accepts
- **Mobile Responsive**: Works seamlessly on desktop and mobile devices
- **Beautiful Animations**: Smooth gradients, transitions, and responsive scaling

## 🛠️ Tech Stack

- **Frontend**: React 18
- **Build Tool**: Vite
- **Styling**: Tailwind CSS + Custom CSS
- **Animations**: CSS animations & transforms
- **Email Service**: EmailJS
- **Package Manager**: npm

## 📝 Prerequisites

- Node.js (v14 or higher)
- npm or yarn
- EmailJS account for sending notifications

## 🚀 Installation

1. Clone the repository:
```bash
git clone https://github.com/Aariyan007/Valentine-day-Special.git
cd Valentine-day-Special
```

2. Install dependencies:
```bash
npm install
```

3. Create a `.env` file in the root directory with your EmailJS credentials:
```bash
VITE_EMAILJS_SERVICE_ID=your_service_id
VITE_EMAILJS_TEMPLATE_ID=your_template_id
VITE_EMAILJS_PUBLIC_KEY=your_public_key
```

4. Start the development server:
```bash
npm run dev
```

5. Open your browser and navigate to the URL shown in the terminal (usually `http://localhost:5173`)

## 🔐 Environment Variables

You need to set up EmailJS credentials:

1. Go to [EmailJS](https://www.emailjs.com/)
2. Sign up for a free account
3. Create a service, template, and get your public key
4. Add these to your `.env` file as shown above

**Important**: The `.env` file should be in the root of your project and will not be committed to Git (it's in `.gitignore`).

## 📦 Build for Production

```bash
npm run build
```

This creates an optimized production build in the `dist` folder.

## 🎨 Customization

You can customize:
- **Questions**: Edit the `questions` array in `src/App.jsx`
- **Colors**: Modify the gradients and colors in inline styles
- **Button Behavior**: Adjust scaling factors and animation timings
- **Email Template**: Customize what gets sent in the `sendEmail` function

## 🌐 Deployment

### Option 1: Vercel (Recommended)
```bash
npm install -g vercel
vercel
```

### Option 2: Netlify
Drag and drop the `dist` folder to [Netlify](https://www.netlify.com/)

### Option 3: GitHub Pages
Update `vite.config.js` with your repository name and run:
```bash
npm run build
npm run deploy
```

## 💝 How It Works

1. **User enters their name** on the welcome screen
2. **Email notification is sent** (optional - user started the app)
3. **Interactive question screen appears** with a charming Valentine's prompt
4. **Clicking "No"** triggers button reactions:
   - "Yes" button grows larger
   - "No" button shrinks and moves around
   - Questions escalate in desperation
5. **Clicking "Yes"** shows a success screen and sends an acceptance notification
6. **Success screen** celebrates the acceptance with emojis and animations

## 📱 Browser Support

Works on all modern browsers:
- Chrome/Edge (latest)
- Firefox (latest)
- Safari (latest)
- Mobile browsers (iOS Safari, Chrome Mobile)

## 🤝 Contributing

Feel free to fork this project and customize it for your own Valentine's Day surprise!

## 📄 License

Free to use for personal projects.

## 💌 Notes

- This app is best experienced on a computer screen for the full button animation effect
- Works great on mobile too, with touch-friendly interactions
- Perfect for social media sharing with a unique link to your deployed version

---

Made with ❤️ for Valentine's Day 2026
