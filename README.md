# Interactive Optics Laboratory

A suite of interactive, browser-based physics simulations designed to visualize core concepts in geometric optics, physical optics, wave acoustics, and polarization. This project serves as an educational tool to bridge the gap between abstract mathematical formulas and visual optical phenomena.

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

### Module 03: Polarization & Wave Plates
This module visualizes the complex phase interactions of polarized light.
* Features an interactive 3D Jones Calculus engine demonstrating linear, circular, and elliptical polarization.
* Explores Malus's Law and waveplate phase shifts using Half-Wave Plates (HWP) and Quarter-Wave Plates (QWP).
* Includes a dynamic 3-way view toggle, allowing users to observe wave propagation via 3D Isometric, Frontal Perspective, or 2D Cross-Section views.
* Incorporates automated, slow-motion presentation presets (5°/sec), including a mathematical breakdown of the "3-Polarizer Paradox".

### Module 04: Acoustics: WaveLab & ANC
This module explores acoustic interference and the DSP mechanics behind Active Noise Cancellation.
* Demonstrates the principle of superposition, beat frequencies, and Fourier harmonics using pure sine, triangle, square, and sawtooth waves.
* Features a "Practical ANC" tab that processes local audio files and live microphone input entirely in-browser.
* Visualizes raw and resultant waveforms using real-time canvas oscilloscopes.
* Simulates real-world ANC hardware limitations, allowing users to introduce DSP calculation latency to observe high-frequency cancellation bleed.
* Includes a "DJ Wobble" preset demonstrating how wave beating creates LFO sub-bass effects.

## 💻 Technical Stack
* Built entirely with HTML5, CSS3, and Vanilla JavaScript.
* Utilizes the HTML5 Canvas API with dynamic High-DPI (Retina display) scaling to ensure mathematically precise, razor-sharp rendering without blurring.
* Integrates the **Web Audio API** (`AudioContext`, `createOscillator`, `createDelay`, `createAnalyser`, and `getUserMedia`) for real-time acoustic signal processing.
* Implements complex number arithmetic for optical state vectors and `requestAnimationFrame` for fluid, continuous hardware-accelerated animations.
* Zero external libraries or dependencies, fully functional offline.

## 🚀 How to Use
1. Clone or download this repository to your local machine.
2. Open `index.html` in any modern web browser to access the main dashboard.
3. Select "Geometric Optics", "Physical Optics", "Polarization & Wave Plates", or "Acoustics: WaveLab & ANC" to launch the respective simulation bench.
4. Use the continuous sliders or direct numerical inputs to manipulate variables and interact with the modules. 

## 👨‍🔬 Author
**Nihal Jonathan Dsouza**  
*M.Sc. in Physics, Manipal Institute of Technology*
