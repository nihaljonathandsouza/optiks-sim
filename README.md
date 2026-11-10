# Interactive Optics & Wave Physics Laboratory

A collection of browser-based educational simulations for exploring geometric optics, physical optics, polarization, wave superposition, Fourier analysis, digital audio and melody construction. The simulations connect mathematical models with interactive visual demonstrations.

The project is intended as a teaching and learning aid. Its optical and audio models use stated idealisations; the simulations are not clinical instruments or substitutes for laboratory measurements.

## Modules

### Module 01: Geometric Optics — Reduced-Eye Refraction

An idealised eye model for exploring image formation and optical correction.

- Visualises ray paths, focal position and retinal focal shift.
- Allows changes to equivalent eye power, axial length, corrective lens power and spectacle vertex distance.
- Calculates vergence at the corneal plane and a model-estimated corrective lens power.
- Includes an adjustable measurement grid and principal/reference-plane display.

**Model limitation:** This is a paraxial reduced-eye teaching model. It does not trace refraction through every anatomical surface of a real eye and must not be used to determine a clinical prescription.

### Module 02: Physical Optics — Diffraction

Interactive demonstrations of diffraction and interference patterns.

- Single-slit diffraction and its intensity distribution.
- Double-slit interference within a single-slit diffraction envelope.
- Circular-aperture diffraction, the Airy pattern and the Rayleigh resolution criterion.
- Monochromatic and multi-wavelength (white-light) diffraction views.
- A separate Newton's Rings thin-film interference illustration and links to laboratory photographs of sodium and mercury light sources.

**Model limitation:** The diffraction patterns use idealised aperture and far-field assumptions. The circular-aperture pupil mode is an optical model, not a complete model of the human eye. Newton's Rings are calculated as a separate thin-film interference system; changing the pupil diameter does not change the Newton's Rings pattern.

### Module 03: Polarization & Wave Plates

An ideal Jones-calculus model for studying the state of polarized light.

- Linear polarizers and Malus's law.
- Half-wave plates (HWP) and quarter-wave plates (QWP).
- Linear, circular and elliptical polarization states.
- Jones-vector and intensity readouts at successive optical elements.
- 3D isometric, frontal and 2D views, along with guided presets.
- A three-polarizer demonstration showing how an intermediate polarizer can allow light through crossed polarizers.

**Model limitation:** The calculation uses ideal optical elements. Unpolarized input is represented by an intensity average at the first polarizer followed by a Jones-vector description of the transmitted, linearly polarized light.

### Module 04: Acoustics — Wave, Fourier & Melody Laboratory

A seven-part interactive laboratory for sound waves, Fourier methods, digital audio and melody construction.

1. **Superposition & Beats:** Combine waveforms, vary amplitude, frequency and phase, and explore constructive/destructive interference and beats.
2. **Fourier Synthesis:** Build a resultant waveform by adjusting the amplitudes of harmonics and compare its time-domain waveform with its harmonic spectrum.
3. **Audio Analyzer:** Load an audio file and inspect its time-domain waveform, FFT frequency spectrum, spectrogram and approximate pitch estimate.
4. **Digital Sampling:** Compare a continuous input with discrete quantised samples and a zero-order-hold output. Change sample rate and bit depth to explore sampling and quantisation effects.
5. **Digital Cancellation:** Add an optional inverted and delayed copy of an audio signal to demonstrate phase cancellation and frequency-dependent effects of delay.
6. **Microphone Loopback:** Use microphone input to explore signal inversion, delay and digital mixing. Microphone access requires browser permission.
7. **Melody Studio:** Explore note sequences, use the on-screen keyboard and song presets, construct custom melodies, change tempo and timbre, and record a performance where supported.

**Important distinction:** The digital cancellation and microphone loopback sections demonstrate digital signal addition and phase cancellation. They are not complete active-noise-cancellation systems: they do not model the acoustic path from a headphone loudspeaker to the listener's ear, adaptive filtering, microphone placement or real headset hardware.

**Model limitations:** The analyzer's pitch readout is an estimate and may be unstable for polyphonic, noisy or inharmonic sounds. The spectrogram and FFT show relative signal levels, not calibrated sound-pressure levels. The sampler illustrates quantisation and sample-and-hold behaviour; it is not a complete analogue-to-digital or digital-to-analogue converter chain with anti-aliasing and reconstruction filters. Fourier synthesis uses a finite set of harmonics, so its waveform presets are approximations.

## Running the Laboratory

1. Download or clone the repository.
2. Keep the dashboard and module files together in the same folder.
3. Start the project using a local web server (for example, VS Code Live Server), or deploy it to a static HTTPS host such as GitHub Pages.
4. Open `index.html` and select the module to launch.

The dashboard currently links to these filenames:

- `refraction.html`
- `diffraction.html`
- `polarization.html`
- `anc.html`

To keep `index.html` unchanged, save the final combined Wave, Fourier & Melody Laboratory as **`anc.html`**. If you prefer to keep the filename `wave_fourier_lab_v3.html`, update the acoustics card link in `index.html` to point to that filename.

Most visual simulations can run locally in a modern browser. The microphone feature requires a secure context (HTTPS or localhost), a compatible browser and the user's permission. A local web server is therefore recommended rather than opening the HTML file directly with `file://`.

## Audio and External Resources

- The audio analyzer accepts locally selected audio files; the selected file is processed in the browser.
- The featured audio-track button in the Wave, Fourier & Melody Laboratory expects an `audio.mp3` file alongside `anc.html`. If that asset is not included, use the local audio-file upload instead.
- Include or redistribute any music or audio assets only when you have the necessary permission. Links to an artist's channel or original track are provided for reference and do not themselves grant redistribution rights.
- Google Fonts are loaded from Google Fonts when an internet connection is available. System fallback fonts are used if the external fonts cannot be reached.

## Technology

- HTML5, CSS3 and vanilla JavaScript.
- HTML Canvas for optical diagrams, waveforms, spectra and spectrograms.
- Web Audio API for oscillator generation, audio playback, analysis, filtering/delay demonstrations and microphone input.
- Browser animation APIs for continuously updated visualisations.

The project does not require a JavaScript framework or a separate backend. Some browser features (especially microphone input and audio playback) depend on browser permissions and support.

## Educational Use

These simulations are designed to support classroom explanations, guided exploration and discussion. Students should compare the visualisations with the equations, assumptions and limitations shown in each module. Where a simulation is idealised, its output should not be interpreted as a clinical measurement or a calibrated laboratory result.

## Author

**Nihal Jonathan Dsouza**
*M.Sc. Physics*
