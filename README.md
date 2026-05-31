# Crypto_Top Website - Multi-Voltage ASIC Design Documentation Portal

A professional, multi-page website for the **Multi-Voltage Crypto Core: RTL to GDSII** project documentation. This is a comprehensive reference portal for a 32nm multi-voltage cryptographic accelerator ASIC design.

## Project Overview

**Multi-Voltage Crypto Core** (Crypto_Top) is a complete RTL-to-GDSII design flow reference that demonstrates:
- **32nm CMOS Technology** with ~600K instances pre-synthesis
- **Dual-voltage architecture** (0.95V high-performance / 0.75V low-power)
- **Complete design flow** from RTL through physical design to signoff
- **Industry-standard methodologies** and tools (Synopsys Design Compiler, ICC2)

## Website Features

### Navigation Structure
- **Home**: Project overview and specifications
- **Input Files**: RTL, UPF, SDC constraints
- **Scripts**: Complete automation flows (Synthesis, Floorplanning, Placement, CTS, Routing, Signoff, DRV/Setup Fixes)
- **Shapes**: Floorplan designs (A Shape, Y Shape)
- **MCMM Constraints**: Multi-corner multi-mode timing setup
- **Manual**: PDF and website documentation links
- **Xtra Files**: Additional resources (coming soon)

### Design Highlights

#### Multi-Voltage Architecture
- **High-Performance Domain (0.95V)**: Main datapath and computational engines
- **Low-Power Domain (0.75V)**: Control logic and peripherals
- Safe voltage-domain crossing with level shifters
- UPF-based power intent integration

#### Complete Design Flow
1. **RTL Design**: 128-bit cryptographic accelerator with SPN architecture
2. **Synthesis**: Multi-voltage synthesis with DFT insertion
3. **Floorplanning**: Core-aware floorplan with voltage areas
4. **Power Planning**: Multi-domain mesh PDN
5. **Placement**: Congestion-aware optimization
6. **Clock Tree Synthesis**: Low-skew clock distribution with level shifting
7. **Routing**: Timing and SI-driven routing
8. **Signoff**: Parasitic extraction and PrimeTime analysis

#### ECO Techniques
- Automated cell upsizing for max transition fixes
- Buffer insertion for max capacitance fixes
- Dynamic voltage-area generation

## File Structure

```
crypto_top Website/
├── index.html                 # Main website (all pages integrated)
├── css/
│   └── styles.css             # Professional styling with responsive design
├── js/
│   └── script.js              # Navigation and page management
├── pages/                     # (Optional) Individual page templates
└── README.md                  # This file
```

## Design & Styling

### Color Scheme
- **Primary**: Deep blue (#1a1a2e)
- **Secondary**: Navy (#16213e)
- **Accent**: Slate blue (#0f3460)
- **Highlight**: Crimson red (#e94560)

### Features
- **Responsive Design**: Works on desktop, tablet, and mobile
- **Sticky Navigation**: Easy access to all sections
- **Smooth Animations**: Professional fade-in transitions
- **Professional Typography**: Segoe UI with clean hierarchy
- **Accessible Layout**: Proper semantic HTML structure

### Responsive Breakpoints
- **Desktop**: Full layout with side-by-side content
- **Tablet (≤1024px)**: Optimized grid columns
- **Mobile (≤768px)**: Hamburger menu, single column layout
- **Small Mobile (≤480px)**: Simplified navbar and text sizes

## Getting Started

### Quick Start
1. Open `index.html` in a web browser
2. Navigate using the horizontal navbar
3. Explore all pages and sections

### Local Development
```bash
# No build process required - this is a static website
# Simply open index.html in your browser or use a local server:

# Using Python 3
python -m http.server 8000

# Using Node.js http-server
npx http-server .

# Using VS Code Live Server extension
# Right-click index.html → "Open with Live Server"
```

## Content Sections

### Home Page
- Project title and overview
- Technology specifications table
- Project architecture and voltage domains
- Multi-voltage design challenges
- Copyright and legal information

### Input Files
- **RTL**: 128-bit cryptographic accelerator design
- **UPF**: Multi-voltage power intent specification
- **SDC**: Synthesis and physical design timing constraints

### Scripts
- **Synthesis**: Synopsys Design Compiler flow with DFT
- **Floorplan-to-Powerplan**: Physical design initialization
- **Placement**: Placement optimization setup
- **Clock Tree Synthesis**: CTS for multi-voltage design
- **Routing**: Timing-driven routing with SI awareness
- **Signoff**: Parasitic extraction and STA handoff
- **DRV Fixes**: Cell upsizing and buffer insertion
- **Setup Fixes**: Voltage area creation and floorplan iteration

### Shapes
- **A Shape**: Core floorplan initialization and design
- **Y Shape**: Floorplan iteration and congestion analysis

### Other Sections
- **MCMM Constraints**: Multi-corner multi-mode timing analysis
- **Manual**: Links to PDF and website documentation
- **Xtra Files**: Additional resources (coming soon)

## Technology Stack

- **HTML5**: Semantic structure and accessibility
- **CSS3**: Modern styling with gradients, animations, and flexbox/grid
- **JavaScript (Vanilla)**: Navigation, page switching, and interactivity

## Compatibility

### Browsers
- Chrome/Chromium (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)

### Operating Systems
- Windows 10/11
- macOS
- Linux
- iOS/Android (mobile browsers)

## Features

### Navigation
- **Sticky Navbar**: Always accessible horizontal navigation
- **Submenu Support**: Dropdown menus for nested pages
- **Mobile Menu**: Hamburger menu on smaller screens
- **Hash-based Routing**: Clean URLs without server-side routing

### User Experience
- **Smooth Scrolling**: Elegant scroll behavior throughout
- **Responsive Images**: Proper scaling on all devices
- **Professional Footer**: Contact info, social links, and project metadata
- **Clear Hierarchy**: Well-organized content with proper heading levels

### Accessibility
- **Semantic HTML**: Proper document structure
- **Color Contrast**: High contrast for readability
- **Responsive Design**: Mobile-friendly layout
- **Link Previews**: Clear indication of external links

## Customization

### Changing Colors
Edit CSS variables in `css/styles.css`:
```css
:root {
  --primary-color: #1a1a2e;
  --secondary-color: #16213e;
  --accent-color: #0f3460;
  --highlight-color: #e94560;
  /* ... more colors ... */
}
```

### Adding New Pages
1. Add new `<div class="page" id="new-page">` to index.html
2. Add corresponding navbar link with `data-page="new-page"`
3. Content will automatically be handled by JavaScript navigation

### Modifying Navigation
Edit navbar items in `index.html`:
```html
<li>
    <a href="#page-id" data-page="page-id">Page Name</a>
</li>
```

## Project Information

**Author**: Ajay Mallesh  
**Reviewer**: Gemini Pro 3.1 & Ajay Mallesh  
**Version**: 2.0 (2026)  
**Date**: 23/05/2026

**Email**: ajaymalavalli912@gmail.com  
**LinkedIn**: www.linkedin.com/in/ajaymallesh  
**GitHub**: https://github.com/Ajay-Mallesh

## License

© 2026 Ajay Mallesh. This project is open-source and released for educational and non-commercial community use.

## Legal Disclaimer

The methodologies, TCL examples, UPF constructs, synthesis flows, timing constraints and physical implementation strategies described in this documentation are intended exclusively for educational and research purposes.

The author assumes no responsibility for: silicon failure, timing closure loss, LVS/DRC violations, power collapse, EM degradation, tape-out delay, or fabrication loss arising from improper application of the concepts described herein.

## References

- **GitHub Repository**: https://github.com/Ajay-Mallesh/crypro_top_Project_Files
- **PDF Manual**: Available in repository
- **Website Manual**: https://ajay-mallesh.github.io/crypro_top_manual_website/

## Support

For questions, issues, or contributions:
- Visit the GitHub repository
- Contact the author via email or LinkedIn
- Review the comprehensive documentation in the manual sections

---

**Last Updated**: 31/05/2026  
**Website Version**: 1.0.0
