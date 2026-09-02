# Fungal Biosignal Sonification and Generative Visualisation

This repository contains the data-analysis outputs, sonification experiments, and audiovisual prototype developed for a project exploring how fungal electrical signals can be translated into sound and generative mycelium-inspired visuals.

## Project Overview

The project investigates a pipeline from fungal biosignal data to audiovisual representation:

1. **Fungal electrical signal data**
2. **Signal inspection and processing**
3. **Baseline removal / detrending**
4. **Event detection and feature exploration**
5. **Sonification**
6. **Generative mycelium visualisation**
7. **Integrated audiovisual prototype**

The current prototype uses prerecorded fungal signal data. Future development may connect the pipeline to live Fungi Kit acquisition and user interaction.

## Repository Structure

```text
.
├── Fungi_sound/
│   ├── fungi_sonification_v1.wav
│   └── fungi_sonification_v2_ambient.wav
│
├── Prototype/
│   └── prototype01_growing_mycelium_with_audio.html
│
├── mushroom_results_csvdata/
│   ├── 01_full_recording.png
│   ├── 02_signal_and_baseline.png
│   ├── 03_detrended_signal.png
│   ├── 04_detected_events.png
│   ├── 05_zoom_84_to_88_min.png
│   ├── 06_zoom_129_to_134_min.png
│   ├── 07_zoom_144_to_150_min.png
│   ├── 08_zoom_199_to_204_min.png
│   ├── analysed_mushroom_data.csv
│   ├── detected_mushroom_events.*
│   ├── event_*.*
│   ├── fungi_data_test.csv
│   └── ...
│
└── README.md
```

> Some filenames may appear abbreviated in the file browser. The structure above lists the main artefacts visible in the project folder.

## Folder Description

### `Fungi_sound/`

Contains the audio outputs generated from fungal biosignal data.

- **`fungi_sonification_v1.wav`**  
  Initial fungal-data sonification prototype.

- **`fungi_sonification_v2_ambient.wav`**  
  A second sonification iteration exploring a more ambient and atmospheric sound treatment.

These files document the development of the signal-to-sound mapping and provide evidence of iterative prototyping.

### `Prototype/`

Contains the integrated audiovisual prototype.

- **`prototype01_growing_mycelium_with_audio.html`**  
  Browser-based prototype combining fungal-data sonification with a generative Growing Mycelium visualisation.

The prototype synchronises visual growth behaviour with audio-derived events and includes basic playback controls.

Current visual mappings include:

- audio onset → mycelium growth event
- signal / event strength → branch length
- audio volume → glow and branch thickness
- pitch → growth direction

Open the HTML file in a modern web browser to run the prototype.

### `mushroom_results_csvdata/`

Contains processed fungal-signal data and visual outputs from the analysis workflow.

Key outputs include:

- **`01_full_recording.png`** — overview of the full recording
- **`02_signal_and_baseline.png`** — signal compared with estimated baseline
- **`03_detrended_signal.png`** — signal after baseline removal / detrending
- **`04_detected_events.png`** — detected signal events
- **`05–08_zoom_*.png`** — detailed views of selected time windows
- **`analysed_mushroom_data.csv`** — processed analysis data
- **`detected_mushroom_events.*`** — detected-event results
- **`event_*.*`** — individual event outputs
- **`fungi_data_test.csv`** — fungal signal dataset used for testing / analysis

The zoom plots are used to inspect local signal behaviour and identify potentially meaningful changes before sonification.

## Current Technical Progress

- [x] Fungal signal dataset exploration
- [x] Full-recording visualisation
- [x] Baseline inspection and detrending
- [x] Event detection
- [x] Selected signal-window analysis
- [x] Sonification Prototype 01
- [x] Ambient Sonification Prototype 02
- [x] Generative mycelium visual experiment
- [x] Integrated audiovisual HTML prototype
- [ ] Live Fungi Kit signal acquisition
- [ ] Real-time audiovisual mapping
- [ ] User–fungus interaction prototype
- [ ] Formal evaluation

## Tools and Technologies

The project currently uses or produces artefacts associated with:

- Python
- Jupyter Notebook
- CSV time-series data
- Pandas / NumPy
- Matplotlib
- WAV audio
- HTML5
- JavaScript
- HTML5 Canvas
- HTML Audio
- Browser-based generative visualisation

Future versions are intended to connect the software pipeline to a Fungi Kit hardware acquisition system for live fungal electrical signals.

## Running the Audiovisual Prototype

1. Open the `Prototype/` folder.
2. Open `prototype01_growing_mycelium_with_audio.html` in a modern browser.
3. Select **Play** to start the synchronised audio and mycelium visualisation.
4. Select **Restart** to replay the prototype from the beginning.

No installation is required for the current standalone HTML prototype.

## Current Prototype Boundary

The current working pipeline is:

```text
Prerecorded fungal data
        ↓
Signal analysis
        ↓
Sonification
        ↓
Synchronised generative mycelium visualisation
```

The planned future pipeline is:

```text
User interaction
        ↓
Living fungus
        ↓
Live electrical signal acquisition
        ↓
Signal processing
        ↓
Audiovisual mapping
        ↓
Sound + generative mycelium feedback
```

## Notes

- The current audiovisual prototype uses prerecorded data rather than live fungal input.
- The mapping from biosignal features to sound and visual parameters is a design interpretation rather than a unique biological translation.
- Signal noise, baseline drift, electrode placement, grounding, and environmental interference are important considerations for future real-time implementation.

## Project Status

**Current stage:** working audiovisual prototype with prerecorded fungal biosignal data.

**Next stage:** connect live Fungi Kit acquisition and prototype a closed interaction loop between user action, fungal response, and audiovisual feedback.
