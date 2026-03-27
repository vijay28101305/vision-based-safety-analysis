# Vision-Based Safety & Accessibility Analysis

## Overview
This project builds an image-based system that analyzes safety hazards and accessibility risks from a single image using a vision–language model.

Instead of acting as a black-box AI, the system is designed to be **interpretable and deterministic**, providing structured safety insights that can assist human decision-making.

---

## Problem
Safety inspections in real-world environments (workspaces, streets, public areas) are often:
- Manual and time-consuming  
- Subjective and inconsistent  
- Dependent on human judgment  

This project aims to automate the **initial safety and accessibility analysis** while keeping the results transparent and explainable.

---

## What I Built
- End-to-end vision-language pipeline  
- Image captioning using BLIP model  
- Rule-based scene classification system  
- Deterministic hazard & accessibility reasoning module  
- Structured safety reports (JSON format)  
- Interactive UI using Gradio  

---

## How It Works

### 1. Image Input
User uploads an image through the interface.

### 2. Image Captioning
- Uses a pretrained vision–language model (BLIP)
- Generates a natural language description of the image

### 3. Scene Classification
- Applies keyword-based rules on the caption  
- Assigns scene types like:
  - workspace
  - street
  - park
  - beach  

### 4. Hazard & Accessibility Analysis
- Selects predefined templates based on scene type  
- Generates structured outputs including:
  - Safety hazards  
  - Accessibility risks  
  - Tripping/fall dangers  
  - Environmental conditions  
  - Corrective actions  

### 5. Output
Displays:
- Caption  
- Scene type  
- Structured hazard report  

---

## Example Output
The system produces a structured report with categories such as:
- Safety Hazards  
- Accessibility Risks  
- Wheelchair Accessibility Issues  
- Obstacles or Narrow Pathways  
- Corrective Actions  

---

## Key Design Choices
- **Interpretability over complexity**  
- **Rule-based classification for transparency**  
- **Template-driven reasoning for consistency**  
- **Modular pipeline for easy debugging and extension**  

---

## Results
- Generates consistent and interpretable safety reports  
- Works across multiple environments (indoor and outdoor)  
- Demonstrates strong qualitative performance  

---

## Challenges
- Caption quality affects downstream reasoning  
- Rule-based classification can miss edge cases  
- Templates limit flexibility of hazard detection  

---

## Limitations
- No quantitative risk scoring  
- Limited to static images  
- Not adaptive to unseen complex scenarios  

---

## Future Improvements
- Replace rule-based classification with learned models  
- Extend to video-based hazard detection  
- Integrate real-world safety standards  
- Deploy as mobile or web application  
- Add more advanced reasoning capabilities  

---

## Tech Stack
- Python  
- PyTorch  
- Hugging Face Transformers  
- BLIP Vision-Language Model  
- Pillow (PIL)  
- Gradio  

---

## How to Run

1. Install dependencies:
```bash
pip install -r requirements.txt
```

2. Run the notebook:
```bash
Open the .ipynb file and run all cells
```

---

## Project Structure
```
.
├── notebook.ipynb
├── requirements.txt
└── README.md
```

---

## Conclusion
This project demonstrates how vision–language models can be combined with rule-based reasoning to build an interpretable and practical safety analysis system. It highlights the importance of explainable AI in real-world applications where transparency matters.
