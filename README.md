# FretFlow: The Pentatonic Map 🎸

<img width="1205" height="803" alt="image" src="https://github.com/user-attachments/assets/1da12b98-252f-46cb-9323-843831d5a511" />


FretFlow is an interactive, mobile-friendly web application designed to help guitarists master the **Pentatonic Scale** and connect it to the **CAGED System** across the entire fretboard. Visualize scale patterns, key relationships, and root notes instantly.

## Key Features

* **Dynamic Fretboard:** Visualize any Major or Minor Pentatonic scale on a 24-fret guitar neck.
* **CAGED System Integration:** Isolate and highlight the five essential Pentatonic CAGED shapes: **E, D, C, A, and G**. This helps users understand how the shapes connect seamlessly.
* **Key and Scale Selection:** Choose any key from C to B and switch between **Major** and **Minor** Pentatonic scales.
* **Root Note Highlighting:** The root notes of the selected scale are visually distinct, often marked with a bright yellow border, providing an immediate anchor point.
* **Relative Scale Display:** Instantly shows the relative Major or Minor key that shares the same set of notes (e.g., C Major Pentatonic is the same as A Minor Pentatonic).
* **Note Name Toggle:** Option to display the actual note names (C, D, E, etc.) on the highlighted dots for better musical understanding.
* **Responsive and Scrollable:** The fretboard is horizontally scrollable, allowing exploration of the entire neck, and the interface is built with Tailwind CSS for a modern, dark-mode look.

<img width="1195" height="555" alt="image" src="https://github.com/user-attachments/assets/272c1018-6658-4391-8792-5cf56d9c5812" />




## How It Works

The app uses the following logic to map the scales and shapes:

1.  **Scale Calculation:** Determines the five notes of the chosen scale (Major: R-2-3-5-6; Minor: R-m3-4-5-m7) based on the selected root key.
2.  **Root Position on Fretboard:** Finds the selected Major Pentatonic root note's position on the Low E (6th) string.
   
    <img width="89" height="71" alt="image" src="https://github.com/user-attachments/assets/3a0c03c3-c988-473b-84ff-2dfd6d59cad9" />

4.  **CAGED Box Mapping:** All five CAGED shapes are defined by specific fret ranges relative to that Low E root position. When a shape is selected, only the scale notes that fall within that specific fret range (or its octave repetition) are highlighted in a bright green.
5.  **Interactive Controls:** Updates in real-time as you select a new key, scale type, or CAGED shape.
