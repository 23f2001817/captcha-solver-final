# Captcha Solver

A web-based captcha solver application that handles image URL parameters and displays captcha images with simulated text extraction.

## 🚀 Live Demo

**GitHub Pages URL:** https://23f2001817.github.io/captcha-solver-interactive-test/

Test with a sample image URL:
```
https://23f2001817.github.io/captcha-solver-interactive-test/?url=https://dummyimage.com/300x100/0066cc/ffffff&text=TEST
```

## 📋 Features

- **URL Parameter Support**: Pass captcha image URLs via `?url=IMAGE_URL` parameter
- **Dynamic Image Display**: Automatically loads and displays captcha images from provided URLs
- **Fallback Images**: Uses default sample images when no URL is provided or when images fail to load
- **Responsive Design**: Clean, mobile-friendly interface with modern styling
- **Error Handling**: Graceful handling of broken or invalid image URLs
- **Cross-Origin Support**: Works with various image hosting services
- **Loading States**: Visual feedback during image loading and processing
- **Fast Processing**: Displays solved captcha text within 15 seconds

## 🛠️ Technology Stack

- **Frontend**: HTML5, CSS3, JavaScript (ES6+)
- **Styling**: Modern CSS with flexbox and gradient backgrounds
- **Deployment**: GitHub Pages with automated deployment
- **Version Control**: Git with GitHub integration

## 📖 Usage

### Basic Usage
1. Visit the GitHub Pages URL
2. The app will display a captcha image
3. Pass custom image URLs using the `url` parameter:
   ```
   ?url=YOUR_IMAGE_URL
   ```

### Example URLs
```bash
# Using dummyimage.com
?url=https://dummyimage.com/300x100/0066cc/ffffff&text=SAMPLE

# Using placehold.co
?url=https://placehold.co/300x100/6366f1/white/png?text=CAPTCHA

# Using fakeimg.pl
?url=https://fakeimg.pl/300x100/667eea/ffffff/?text=DEMO

# Default behavior (no parameters)
# Shows the built-in sample image
```

## 🏗️ Setup and Installation

### Local Development
1. Clone the repository:
   ```bash
   git clone https://github.com/23f2001817/captcha-solver-interactive-test.git
   cd captcha-solver-interactive-test
   ```

2. Open `index.html` in your browser or use a local web server:
   ```bash
   # Using Python 3
   python -m http.server 8000
   
   # Using Node.js (with http-server)
   npx http-server
   ```

3. Navigate to `http://localhost:8000` in your browser

### GitHub Pages Deployment
The application is automatically deployed to GitHub Pages when changes are pushed to the main branch.

## 🔧 How It Works

1. **URL Parameter Parsing**: JavaScript extracts the `url` parameter from the current page URL using URLSearchParams
2. **Image Loading**: The application dynamically sets the image source based on the provided URL
3. **Fallback Strategy**: If an image fails to load, the application tries multiple fallback images before showing an error
4. **Simulation**: Provides simulated captcha text extraction with realistic timing delays (1.5-3.5 seconds)
5. **User Interface**: Modern, responsive design with loading states and user feedback

## 🐛 Troubleshooting

### Image Not Loading
- **CORS Issues**: Some image hosts may block cross-origin requests
- **URL Format**: Ensure the image URL is properly encoded and accessible
- **File Type**: Verify the URL points to a valid image file (PNG, JPG, GIF, WebP, etc.)
- **Network Issues**: Check your internet connection and try refreshing

### Recommended Image Services
- ✅ dummyimage.com - Reliable and CORS-friendly
- ✅ placehold.co - Fast and modern
- ✅ fakeimg.pl - Good compatibility

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 👨‍💻 Author

**Kavya S**
- GitHub: [@23f2001817](https://github.com/23f2001817)
- Email: 23f2001817@ds.study.iitm.ac.in

## 🤝 Contributing

Contributions, issues, and feature requests are welcome! Feel free to check the issues page.

## ⭐ Show Your Support

Give a ⭐️ if this project helped you!

---

*Built with ❤️ for the LLM Code Deployment project*
