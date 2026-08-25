# Interactive Optics Laboratory

A suite of interactive, browser-based physics simulations designed to visualize core concepts in geometric and physical optics. This project serves as an educational tool to bridge the gap between abstract mathematical formulas and visual optical phenomena.

## 🔬 Modules

### Module 01: Geometric Optics (Refraction)
This module explores optical correction and lens dynamics using a simplified physiological model.
* Explores ray tracing, refractive errors (Myopia & Hyperopia), and effective lens power dynamics using a reduced eye model.
* Features an "Auto-Refract" tool to calculate exact corrective lens powers based on axial length and vertex distance.
* Calculates real-time vergence math, effective corneal power, and retinal focal shifts.

### Module 02: Physical Optics (Diffraction)
This module visualizes wave interference and the physical limits of optical resolution.
* Visualizes wave interference for single slit and double slit diffraction.
* Simulates the Airy disk and the Rayleigh criterion for optical resolution using circular apertures (pupils).
* Features a broad-spectrum "White Light" mode that demonstrates chromatic dispersion and the formation of spectral rainbows.
* Renders real-time 1D intensity profiles alongside 2D front projections.
* Provides a physical comparison between diffraction-based Airy's Disks and thin-film interference Newton's Rings.
* Includes links to actual laboratory photo captures of Sodium and Mercury light sources for real-world comparison.

## 💻 Technical Stack
* Built entirely with HTML5, CSS3, and Vanilla JavaScript.
* Utilizes the HTML5 Canvas API with dynamic High-DPI (Retina display) scaling to ensure mathematically precise, razor-sharp rendering without blurring.
* Zero external libraries or dependencies, fully functional offline.
* Implements numerical integration algorithms directly in JavaScript to map Bessel functions for 2D circular apertures.

## 🚀 How to Use
1. Clone or download this repository to your local machine.
2. Open `index.html` in any modern web browser to access the main dashboard.
3. Select either "Geometric Optics" or "Physical Optics" to launch the respective simulation bench.
4. Use the sliders to manipulate variables like wavelength, aperture size, and vertex distance. 

## 👨‍🔬 Author
**Nihal Jonathan Dsouza**  
*M.Sc. in Physics, Manipal Institute of Technology*
