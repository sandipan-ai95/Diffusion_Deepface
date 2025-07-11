
## Project Title: Quality Controlled Human Face Synthesis Using Diffusion and DeepFace

### Description:
Generate human face images conditioned on multiple attributes like gender, age, and emotion using Stable Diffusion and DeepFace filtering. Ensures quality-controlled dataset creation by filtering generated images based on analysis.

### Technical Architecture:
- **Stable Diffusion Pipeline:** Generates high-resolution face portraits with adjustable prompts.
- **DeepFace Analysis:** Validates generated faces based on:
  - Gender detection with confidence scores.
  - Age prediction.
  - Emotion detection with threshold control.
- **Filtering Logic:**
  - Only images meeting all three conditions (gender, age range, emotion with confidence threshold) are saved.
  - Processed in batches for efficiency.
- **Output Management:**
  - Filtered images saved to `filtered_faces` directory.
  - Logs printed to console for validation insight.

### Features:
- Stable Diffusion-based face generation.
- DeepFace validation for gender, age, and emotion.
- Saves only valid, quality-controlled images.
- Adjustable parameters: gender, age range, emotion.

  <img width="512" height="512" alt="image" src="https://github.com/user-attachments/assets/87fb62ee-bf91-4f7f-bd84-278564800657" />


### Installation:
```bash
pip install -r requirements.txt
```

### Usage:
Run the script in your preferred Python environment (Colab recommended for GPU access).

### Author:
Sandipan Das

### Disclaimer:
For educational and research use only. Ensure ethical and responsible use.

"""
