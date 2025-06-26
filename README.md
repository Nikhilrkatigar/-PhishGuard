# 🛡️ PhishGuard - URL Security Scanner

> Advanced phishing detection and URL security analysis tool built with modern web technologies


[![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat&logo=html5&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/HTML)
[![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat&logo=css3&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/CSS)
[![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat&logo=javascript&logoColor=black)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)

## 📋 Table of Contents

- [Overview](#overview)
- [Features](#features)
- [Demo](#demo)
- [Installation](#installation)
- [Usage](#usage)
- [Detection Mechanisms](#detection-mechanisms)
- [Risk Scoring System](#risk-scoring-system)
- [Screenshots](#screenshots)
- [Contributing](#contributing)
- [License](#license)
- [Support](#support)

## 🔍 Overview

PhishGuard is a comprehensive client-side URL security scanner that helps users identify potentially malicious websites and phishing attempts. Built entirely with vanilla HTML, CSS, and JavaScript, it provides real-time analysis without requiring any server-side processing, ensuring user privacy and fast response times.

### Why PhishGuard?

- **🔒 Privacy-First**: All analysis happens locally in your browser
- **⚡ Real-Time Scanning**: Instant results with sophisticated pattern recognition
- **🎯 Comprehensive Detection**: Multiple layers of security analysis
- **📊 Risk Scoring**: Clear, actionable security assessments
- **📱 Responsive Design**: Works seamlessly across all devices

## ✨ Features

### Core Security Features
- 🌐 **Domain Analysis** - Examines domain structure, age patterns, and reputation indicators
- 🔒 **HTTPS Verification** - Checks for secure connection protocols
- 🎭 **Homograph Attack Detection** - Identifies character substitution attacks
- 📝 **Keyword Analysis** - Scans for suspicious phishing-related terms
- 🔗 **URL Pattern Recognition** - Analyzes suspicious URL structures and encoding
- 🏷️ **TLD Reputation Checking** - Evaluates top-level domain safety
- 🔍 **Shortener Detection** - Identifies potentially obfuscated URLs

### User Experience Features
- 📊 **Personal Dashboard** - Track your scanning history and statistics
- 📈 **Risk Scoring** - Clear 0-100 risk assessment scale
- 🎨 **Modern UI/UX** - Glassmorphism design with smooth animations
- 📱 **Mobile Responsive** - Optimized for all screen sizes
- 🌙 **Loading Animations** - Skeleton screens and smooth transitions
- 📝 **Scan History** - Keep track of previously analyzed URLs

## 🚀 Demo

Try PhishGuard live: [Demo Link](your-demo-link-here)

## 📦 Installation

### Option 1: Direct Download
1. Download or clone this repository
```bash
git clone https://github.com/yourusername/phishguard.git
cd phishguard
```

2. Open `index.html` in your web browser
```bash
# On macOS
open index.html

# On Windows
start index.html

# On Linux
xdg-open index.html
```

### Option 2: Local Web Server
For the best experience, serve the files through a local web server:

```bash
# Using Python 3
python -m http.server 8000

# Using Node.js (http-server)
npx http-server

# Using PHP
php -S localhost:8000
```

Then visit `http://localhost:8000`

### Option 3: Deploy to GitHub Pages
1. Fork this repository
2. Go to Settings → Pages
3. Select source branch (usually `main`)
4. Your PhishGuard instance will be available at `https://yourusername.github.io/phishguard`

## 🎯 Usage

### Basic Scanning
1. **Enter URL**: Input any URL in the scanner field
2. **Click Scan**: Hit the "Scan for Threats" button
3. **Review Results**: Analyze the risk score and detailed indicators
4. **Check History**: View your scanning history in the Profile section

### Understanding Risk Scores
- **0-20**: 🟢 **Low Risk** - Generally safe with standard security measures
- **21-50**: 🟡 **Medium Risk** - Proceed with caution, verify legitimacy
- **51-100**: 🔴 **High Risk** - Potentially dangerous, avoid interaction

### Example URLs to Test
```
# Safe URLs
https://google.com
https://github.com
https://stackoverflow.com

# Potentially Suspicious Patterns
http://secure-bank-login.tk
https://paypal-verify-account.com
http://192.168.1.1/login
```

## 🔧 Detection Mechanisms

PhishGuard employs multiple detection layers to provide comprehensive security analysis:

### 1. Protocol Security Analysis
- Checks for HTTPS implementation
- Validates secure connection protocols
- Identifies mixed content issues

### 2. Domain Reputation Assessment
```javascript
// Suspicious TLD detection
const suspiciousTlds = ['.tk', '.ml', '.ga', '.cf', '.pw', '.top'];
```

### 3. Pattern Recognition Engine
- **Homograph Attacks**: Detects character substitution using similar-looking characters
- **Typosquatting**: Identifies domains mimicking legitimate sites
- **Keyword Analysis**: Scans for phishing-related terms

### 4. URL Structure Analysis
- Excessive subdomain detection
- URL encoding analysis
- IP address usage instead of domain names
- Suspicious URL schemes

### 5. Heuristic Analysis
- Domain length assessment
- URL shortener detection
- Suspicious keyword combinations

## 📊 Risk Scoring System

PhishGuard uses a weighted scoring algorithm that assigns risk points based on various threat indicators:

| Risk Factor | Points | Description |
|-------------|--------|-------------|
| No HTTPS | +20 | Unencrypted connection |
| Suspicious TLD | +30 | High-risk top-level domain |
| URL Shortener | +25 | Destination unclear |
| Suspicious Keywords | +15 each | Phishing-related terms |
| Excessive Subdomains | +15 | Complex domain structure |
| Homograph Attack | +40 | Character substitution |
| IP Address Usage | +35 | No legitimate domain |
| Malicious Scheme | +50 | Dangerous URL scheme |



## 🛠️ Technical Details

### Architecture
- **Frontend**: Vanilla HTML5, CSS3, JavaScript (ES6+)
- **Storage**: LocalStorage for scan history
- **Design**: Modern glassmorphism with CSS Grid/Flexbox
- **Animations**: CSS transitions and keyframe animations

### Browser Compatibility
- ✅ Chrome 60+
- ✅ Firefox 55+
- ✅ Safari 12+
- ✅ Edge 79+

### File Structure
```
phishguard/
├── index.html          # Main application file
├── README.md          # Project documentation
├── LICENSE            # MIT License
├── screenshots/       # Application screenshots
│   ├── scanner.png
│   ├── results.png
│   ├── profile.png
│   └── about.png
└── docs/             # Additional documentation
    └── CONTRIBUTING.md
```

## 🤝 Contributing

We welcome contributions to PhishGuard! Here's how you can help:

### Ways to Contribute
- 🐛 **Bug Reports**: Found an issue? Let us know!
- ✨ **Feature Requests**: Have ideas for improvements?
- 🔧 **Code Contributions**: Submit pull requests
- 📖 **Documentation**: Help improve our docs
- 🧪 **Testing**: Test with different URLs and scenarios

### Development Setup
1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Make your changes
4. Test thoroughly
5. Commit your changes (`git commit -m 'Add amazing feature'`)
6. Push to the branch (`git push origin feature/amazing-feature`)
7. Open a Pull Request

### Coding Standards
- Use consistent indentation (2 spaces)
- Add comments for complex logic
- Follow semantic HTML structure
- Use CSS custom properties for theming
- Write descriptive commit messages


## 🆘 Support

### Getting Help
- 📖 **Documentation**: Check our [Wiki](../../wiki)
- 🐛 **Bug Reports**: [Issue Tracker](../../issues)
- 💬 **Discussions**: [GitHub Discussions](../../discussions)
- 📧 **Email**: support@phishguard.dev

### Common Issues

**Q: The scanner isn't working in my browser**
A: Ensure you're using a modern browser and that JavaScript is enabled.

**Q: Can I add custom detection rules?**
A: Currently, detection rules are built-in, but we're working on a plugin system.

**Q: Is my scan data sent to any servers?**
A: No! All analysis happens locally in your browser for maximum privacy.

**Q: How accurate is the detection?**
A: PhishGuard uses heuristic analysis and may have false positives. Always use your judgment.

## 🚨 Disclaimer

PhishGuard is a security tool designed to assist users in identifying potentially malicious URLs. While we strive for accuracy, no automated system is 100% perfect. Always exercise caution when browsing the internet and use PhishGuard as one part of your overall security strategy.

**Important Notes:**
- This tool provides heuristic analysis, not definitive security assessments
- False positives and negatives are possible
- Always verify suspicious results through multiple sources
- Keep your browser and security software updated

## 🌟 Acknowledgments

- Thanks to all contributors who help make PhishGuard better
- Inspired by the need for accessible cybersecurity tools
- Built with modern web standards and best practices

---

<div align="center">

**Made with ❤️ for a safer internet**

[⭐ Star this repo](../../stargazers) • [🍴 Fork it](../../fork) • [📝 Report issues](../../issues) • [💬 Discussions](../../discussions)

</div>
