# 🌌 Space Travel Adventures

> An interactive static website showcasing space travel destinations with dynamic content powered by GitHub Actions.

![Space Travel](https://img.shields.io/badge/Space-Travel-blue) ![GitHub Pages](https://img.shields.io/badge/GitHub-Pages-brightgreen) ![Static Site](https://img.shields.io/badge/Static-Site-orange)

## 🚀 Live Demo

Visit the live website: **[https://vstrog.github.io/planets/](https://vstrog.github.io/planets/)**

## 📖 Overview

**Space Travel Adventures** is an interactive static website that allows users to explore different space travel destinations including the Moon, Mars, Mercury, Venus, International Space Station, Jupiter, and Saturn. The unique feature of this project is its integration with GitHub Actions - the default displayed planet can be changed through GitHub workflow dispatches, making it a great example of CI/CD for static sites.

### Key Features:
- 🌍 **7 Space Destinations**: Explore detailed information about each celestial body
- 🎨 **Dynamic Theming**: Automatic color scheme changes based on selected planet
- ⚡ **GitHub Actions Integration**: Change default planet via workflow dispatches
- 📱 **Responsive Design**: Works perfectly on desktop and mobile devices
- 🚀 **Interactive UI**: Smooth animations and transitions

## 🛠️ Technologies & Stack

| Technology | Purpose |
|------------|---------|
| **HTML5** | Website structure and semantics |
| **Tailwind CSS** | Utility-first CSS framework for styling |
| **JavaScript (ES6+)** | Dynamic content and interactivity |
| **GitHub Pages** | Static site hosting |
| **GitHub Actions** | CI/CD and automated deployments |
| **Font Awesome** | Icons and visual elements |
| **Google Fonts** | Typography (Orbitron, Exo 2) |

## 📦 Installation & Setup

This is a static website that requires no build process. However, you can set it up locally:

### Quick Local Setup
```bash
# Clone the repository
git clone https://github.com/vstrog/planets.git

# Navigate to the project directory
cd planets

# Open in your browser
open index.html
# or
npx serve .
# or
python -m http.server 8000
```

### For Development
Since this uses Tailwind CSS via CDN, no build process is required. However, if you want to customize styles:

1. Install Tailwind CSS locally:
```bash
npm install -D tailwindcss
npx tailwindcss init
```

2. Update the configuration as needed and build CSS.

## 📁 Project Structure

```
planets/
├── index.html                 # Main website file
├── .github/
│   └── workflows/
│       └── deploy.yml         # GitHub Actions deployment workflow
├── deployment-info.txt        # Auto-generated deployment information
└── README.md                  # Project documentation
```

## ✨ Features

### 🪐 Dynamic Planet Content
- **Real-time Switching**: Change planets using the dropdown selector
- **URL Parameters**: Direct links to specific planets (e.g., `?planet=mars`)
- **Persistent State**: Browser history integration

### 🎨 Visual Design
- **Space-Themed UI**: Dark theme with starry background
- **Planet-Specific Colors**: Each destination has its own color scheme
- **Responsive Layout**: Adapts to all screen sizes
- **Smooth Animations**: CSS transitions and JavaScript animations

### 📊 Information Display
- **Key Facts**: Distance, travel time, gravity, temperature
- **Travel Details**: Cost, available dates, spaceship information
- **Difficulty Metrics**: Visual progress bars for challenge levels
- **Journey Highlights**: Key activities for each destination

### 🔧 GitHub Integration
- **Workflow Dispatch**: Change default planet via GitHub Actions
- **Automated Deployment**: Push to main branch triggers deployment
- **Manual Triggers**: Deploy with specific planet selection

## 🎮 Usage Examples

### Changing Planets via UI
1. Use the dropdown selector in the header
2. Watch the content, colors, and planet visualization update instantly

### Direct Links to Planets
- **Mars**: `https://vstrog.github.io/planets/?planet=mars`
- **ISS**: `https://vstrog.github.io/planets/?planet=iss`
- **Jupiter**: `https://vstrog.github.io/planets/?planet=jupiter`

### GitHub Actions Deployment
1. Go to **Actions** tab in the repository
2. Select **"Deploy to GitHub Pages"** workflow
3. Click **"Run workflow"**
4. Choose your desired default planet
5. Click **"Run workflow"** to deploy

## 🔧 GitHub Actions Workflow

The project includes a CI/CD pipeline that:

- **Automatically deploys** on pushes to main branch
- **Manual deployment** with planet selection
- **Sets default planet** based on workflow input
- **Generates deployment info** with timestamp

### Workflow Input Options:
- 🌙 Moon
- ♂️ Mars
- ☿️ Mercury
- ♀️ Venus
- 🛰️ ISS
- ♃ Jupiter
- ♄ Saturn

## 🌟 Future Enhancements

Potential improvements for the project:

- [ ] Add more celestial bodies (Pluto, asteroids, etc.)
- [ ] Implement 3D planet models using Three.js
- [ ] Add booking simulation functionality
- [ ] Include real NASA API data
- [ ] Add multi-language support
- [ ] Implement PWA features for offline access

## 🤝 Contributing

Contributions are welcome! Here's how you can help:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the [MIT License](./LICENSE).

## ❓ FAQ

### Q: How does the GitHub Actions integration work?
A: The workflow allows you to set a default planet that will be shown when users visit the base URL without parameters. It modifies the HTML during deployment.

### Q: Can I add new planets?
A: Yes! You would need to:
1. Add the planet data to the `planetData` object in JavaScript
2. Update the planet selector dropdown
3. Add corresponding CSS color classes
4. Update the GitHub Actions workflow options

### Q: Is there a build process?
A: No, this is a pure static site. All processing happens in the browser or via GitHub Actions during deployment.

### Q: How can I customize the colors?
A: Modify the CSS variables in the style section for each planet class (`.moon-color`, `.mars-color`, etc.).

## 👨‍💻 Author

**Vstrog**
- GitHub: [@vstrog](https://github.com/vstrog)
- Project: [Space Travel Adventures](https://github.com/vstrog/planets)

---

<div align="center">

### 🌠 Explore the Cosmos!

*"The cosmos is within us. We are made of star-stuff. We are a way for the universe to know itself."* - Carl Sagan

</div>

---

**⭐ Don't forget to star the repository if you like this project!**
