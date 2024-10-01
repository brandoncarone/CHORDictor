# The Jazzy CHORDictor

**A Python Program for Jazz Chord Progression Annotation**

## Overview

The **Jazzy CHORDictor** is a Python-based tool designed to automatically annotate jazz chord progressions from MIDI files. It was developed as part of a **Music Information Retrieval** course project at New York University. The program leverages jazz piano MIDI multitracks and aims to explore how well automated systems can annotate complex jazz harmonies, which often involve "colorful" chords and improvisational elements that differ from the more rigid structures of Western classical music.

The **CHORDictor** uses a human-in-the-loop approach to ensure the highest annotation accuracy. For any ambiguous chords that the model cannot accurately label, it flags them for manual review and correction.

## Project Scope

The project's main objectives are:
- To create a dataset of annotated jazz piano MIDI features that can be used for chord progression prediction tasks.
- To implement an automatic chord annotation pipeline that processes MIDI files and provides annotations for each beat.
- To incorporate a **Hidden Markov Model (HMM)** or another model to predict subsequent chords if time permits.

### Dataset Details
- **Dataset Source**: Jazz Piano MIDI Multitracks from [Doug McKenzie's website](https://bushgrafts.com/midi/)
- **Size**: 310 MIDI files, approximately 20 hours of musical content.
- **Features**: Each file is parsed to extract the piano track, and the notes are mapped to chord labels using MIDI chord templates.

### Install Dependencies
Run the following commands to install the required packages:

```sh
pip install mido
pip install music21
```
