# Asteroid Impact Simulator

## Overview

Asteroid Impact Simulator is an interactive web application that visualizes the effects of asteroid impacts on Earth using real-time map visualization. Users can customize asteroid properties and observe the simulated impact effects on an interactive world map.

## Features

- **Interactive Map Visualization**: Built with Leaflet.js with dark theme styling
- **Customizable Asteroid Properties**: Adjust diameter, speed, angle, and composition
- **Realistic Impact Simulation**: Calculates and displays multiple impact effects:
  - Crater formation and dimensions
  - Energy release in megatons
  - Fireball radius
  - Seismic activity (earthquake magnitude)
  - Destruction radius
  - Ejecta blanket coverage
  - Thermal radiation zone
  - Tsunami generation (for ocean impacts)
- **Audio-Visual Experience**: 
  - Text-to-speech announcements of impact results
  - Sound effects for launch sequence and impact
  - Animated visual effects on map
- **Multiple Composition Types**: Stone, iron, carbon, and gold asteroids with different densities
- **Responsive Design**: Works on desktop and mobile devices

## Technical Implementation

### Core Technologies
- **Leaflet.js** for interactive map visualization
- **Web Audio API** for sound synthesis and effects
- **Web Speech API** for text-to-speech functionality
- **Vanilla JavaScript** for simulation logic
- **CSS3** with animations and gradients for visual effects

### Physics Model
- **Energy Calculation**: Kinetic energy based on mass and velocity
- **Impact Effects**:
  - Crater diameter scaling with energy
  - Fireball radius calculation
  - Seismic magnitude estimation
  - Destruction zone modeling
  - Tsunami height prediction for ocean impacts
- **Material Properties**: Different densities for various asteroid compositions

### Visual Components
- **Animated Asteroid Trajectory**: Moving marker showing approach path
- **Impact Effects**:
  - Explosion animation at impact point
  - Crater visualization
  - Animated damage rings (fireball, thermal, destruction, ejecta, tsunami)
  - Color-coded zones with descriptive popups
- **Interactive Map Features**:
  - Click to set impact location
  - Real-time coordinate display
  - Zoom controls
  - Impact information popups

## Setup and Usage

### Prerequisites
- Modern web browser with JavaScript enabled
- Internet connection for CDN resources (Leaflet, Font Awesome)

### Installation
1. Download or clone the project files
2. Open `index.html` in a web browser
3. No server setup required - runs directly in browser

### Operation Instructions
1. **Set Impact Location**: Click anywhere on the world map
2. **Configure Asteroid**:
   - Adjust diameter (50-5000 meters)
   - Set speed (5-70 km/s)
   - Choose entry angle (10-90 degrees)
   - Select composition (stone, iron, carbon, gold)
3. **Launch Simulation**: Click "LAUNCH ASTEROID" button
4. **Observe Results**:
   - Watch animated approach and impact
   - View damage rings expanding on map
   - Listen to audio announcement of results
   - Read detailed impact metrics in results panel

## File Structure
```
asteroid-impact-simulator/
├── index.html                 # Main application file
├── (CDN resources)            # Leaflet, Font Awesome loaded from CDN
└── (Audio resources)          # Sound effects from external sources
```

## Impact Calculations

### Energy Release
- Calculated from kinetic energy formula: E = ½mv²
- Converted to megaton equivalents for comparison
- Scales with asteroid mass and velocity

### Effect Radii
- **Crater Diameter**: Based on energy scaling laws
- **Fireball Radius**: Thermal radiation zone
- **Destruction Radius**: Complete structural damage
- **Ejecta Radius**: Debris fallout area
- **Thermal Radius**: Severe burns zone
- **Tsunami Height**: For ocean impacts, based on energy

### Composition Effects
- Different material densities affect mass calculation
- Stone: 3 g/cm³
- Iron: 7.8 g/cm³  
- Carbon: 2.2 g/cm³
- Gold: 19.3 g/cm³

## Audio Features

### Text-to-Speech
- Automatic announcement of impact results
- Female voice preference for clarity
- Adjustable speech rate and pitch
- Stop functionality for user control

### Sound Effects
- Launch sequence with frequency sweeps
- Impact explosion synthesis
- Post-impact rumble effects
- Web Audio API for precise timing

## Browser Compatibility
- Chrome 60+
- Firefox 55+
- Safari 11+
- Edge 79+
- Mobile browsers with Web Audio support

## Performance Considerations
- Efficient layer management for map effects
- Automatic cleanup of animation elements
- Optimized audio synthesis
- Responsive design for various screen sizes

## Educational Value
- Demonstrates real-world impact physics
- Visualizes scale of astronomical events
- Provides context for energy comparisons
- Shows geographic consequences of impacts

## License
This project is for educational and demonstration purposes. Please ensure compliance with terms of service for any external resources used.

## Acknowledgments
- Leaflet.js for mapping functionality
- OpenStreetMap for map tiles
- Web Audio API for sound synthesis
- Impact physics based on scientific models
