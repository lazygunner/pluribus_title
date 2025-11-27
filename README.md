Pluribus Title Sequence Recreation

This project uses Web frontend technologies (HTML5 Canvas and vanilla JavaScript) to recreate the opening title sequence effect of the TV show Pluribus.

🚀 Master Prompt for Code Generation

If you wish to generate the final code for this project in one go, please copy the following prompt and send it to the LLM:

**Task Objective**: Recreate the *Pluribus* TV show opening title particle effect using HTML5 Canvas and vanilla JavaScript in a single file.

**Core Features & Visual Requirements:**

1.  **Typography & Font**:
    * Import the `Montserrat` (Black 900) font from Google Fonts.
    * Render the text "PLUR1BUS" in the center of the screen.
    * **Magnetic Texture**: Do not use a standard grid for the text particles. Instead, arrange them based on an **elliptical magnetic field formula** centered on the first letter 'P' (with subtle organic sine wave perturbations), creating a fingerprint-like, centripetal texture.
    * **Negative Space**: Calculate the geometric position of each letter and establish elliptical **exclusion zones** around them. Force background particles to stay out of these zones to ensure sharp, clean text edges.

2.  **Background Particle System**:
    * Generate a high-density grid of white particles covering the full screen.
    * **Physics**: Background particles should behave as a "rigid medium" with extremely high recoil/friction (> 0.85). They should snap back to their original positions instantly after being disturbed, rather than drifting.

3.  **Sonic Wave Simulation**:
    * Emit high-frequency circular physical pulses from the letter 'P' as the epicenter.
    * **Aggregation Effect**: When a wave passes, **do not** push particles away. Instead, strongly **pull** surrounding background particles toward the wave crest, creating high-density compression bands.
    * **Visual Rendering**: Do not draw lines or circles directly. The visualization of the wave should rely entirely on **particle density superposition**. To prevent black gaps caused by physical movement, dynamically inject temporary "ghost particles" at the wave crest. Their size, brightness, and density must be mathematically calculated to blend perfectly with the background particles.
    * **Text Stability**: Text particles should remain virtually unaffected by the physical force of the sonic waves, maintaining stability while exhibiting a constant, subtle electrical noise jitter.

4.  **Audio & Interaction**:
    * Load and loop play `pluribus_music.mp3`.
    * **Autoplay Handling**: Implement a full-screen interactive **Overlay** prompting the user to "Click screen to initialize system". Upon clicking, remove the overlay and start both the audio and the animation to comply with modern browser autoplay policies.

5.  **Code Requirements**:
    * All logic, styles, and structure must be contained within a single HTML file.
    * Ensure performance optimization to smoothly handle the real-time physics calculation of thousands of particles.


📂 Project File Structure

index.html: The single-file source code containing all logic and styles.

pluribus_music.mp3: Background audio file (must be in the same directory as the HTML).
