# Magenet - Secure and Anonymous Internet Access Portal

Magenet is a web-based platform that provides users with free and secure internet access through VPN services. The platform offers a user-friendly interface for VPN setup instructions, a comprehensive knowledge base, and direct support through Telegram.

The platform features a modern, responsive design with smooth animations and a dark theme for better user experience. It includes detailed VPN setup guides, recommended VPN clients, and additional resources like Windows/Office activation guides and ISO downloads. The platform prioritizes user privacy and accessibility while maintaining a clean, professional interface.

## Repository Structure
```
magenet/
├── index.html          # Main landing page with service overview and navigation
├── library.html        # Knowledge base with Windows/Office resources and VPN clients
├── vpn_install.html    # Step-by-step VPN installation guide
└── styles.css         # Global styling with dark theme and animations
```

## Usage Instructions
### Prerequisites
- Modern web browser (Chrome, Firefox, Safari, or Edge)
- Internet connection
- Basic understanding of VPN concepts

### Installation
1. Clone the repository:
```bash
git clone <repository-url>
```

2. Deploy to a web server or open locally:
```bash
# Using Python's built-in server
python -m http.server 8000

# Using Node.js http-server
npx http-server
```

### Quick Start
1. Navigate to `index.html` in your web browser
2. Click "Настройка VPN" for VPN setup instructions
3. Follow the step-by-step guide to:
   - Obtain VPN configuration
   - Install recommended VPN client
   - Configure VPN connection

### More Detailed Examples
#### Accessing the Knowledge Base
1. Click "База знаний" on the main page
2. Browse available sections:
   - Windows/Office activation guides
   - OS image downloads
   - VPN client recommendations

### Troubleshooting
Common Issues:
1. Images not loading
   - Verify image paths in the `img/` directory
   - Check file permissions
   - Ensure proper image formats (PNG/JPG)

2. Styling issues
   - Confirm Bootstrap CDN is accessible
   - Verify `styles.css` is properly linked
   - Clear browser cache

3. Animations not working
   - Check AOS library is properly loaded
   - Verify JavaScript is enabled
   - Console for potential errors

## Data Flow
The website follows a simple static content delivery model with client-side animations and styling.

```ascii
User Request → Web Server → Static Files (HTML/CSS) → Browser Rendering → User Interface
                                                  ↓
                              External Resources (Bootstrap/AOS)
```

Component Interactions:
1. HTML files provide structure and content
2. CSS (styles.css) handles visual presentation
3. Bootstrap provides responsive layout and components
4. AOS library manages scroll animations
5. External links connect to Telegram and download resources
6. Browser handles all rendering and user interactions
7. No server-side processing or database required