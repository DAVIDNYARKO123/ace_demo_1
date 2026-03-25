# AI API Demos

> Hands-on demonstrations of Google Gemini, OpenAI, and Anthropic Claude APIs

## Overview

This project contains three independent Jupyter notebook demos showcasing different capabilities of modern AI APIs:

- **Claude Demo**: Text generation using Anthropic's Claude API
- **OpenAI Demo**: Image generation from text descriptions
- **Gemini Demo**: Object detection with bounding boxes

## Features

### Claude Demo (`main_claude_demo.ipynb`)

- Generate creative tongue-twisters using Claude Sonnet 4.6
- Demonstrates zero-shot and one-shot prompting techniques
- Configurable temperature and token limits

### OpenAI Demo (`main_openai_demo.ipynb`)

- Create realistic images from text descriptions using GPT-5
- Save generated images to the output directory
- Interactive visualization with Plotly

### Gemini Demo (`main_gemini_demo.ipynb`)

- Detect objects in images using Gemini Robotics ER 1.5 Preview
- Returns normalized bounding box coordinates and confidence scores
- Export detection results to CSV
- Visualize detections with annotated images

## Project Structure

```
ace_demo_1/
├── main_claude_demo.ipynb      # Claude text generation demo
├── main_openai_demo.ipynb      # OpenAI image generation demo
├── main_gemini_demo.ipynb      # Gemini object detection demo
├── utils/
│   └── .env.example            # API keys template
├── images/
│   └── coco128_sample/         # Sample test images
├── output/
│   └── openai/                 # Generated images output
├── detections.csv              # Object detection results
└── annotated_image.jpg         # Annotated image with bounding boxes
```

## Setup

### Prerequisites

- Python 3.9 or higher
- Jupyter Notebook or JupyterLab
- API keys for Claude, OpenAI, and Gemini (depending on which demos you want to run)

### Installation

1. Clone the repository:

```bash
git clone https://github.com/DAVIDNYARKO123/ace_demo_1.git
cd ace_demo_1
```

2. Create and activate a virtual environment:

```bash
python -m venv .venv
source .venv/bin/activate
```

### API Configuration

Create a `.env` file in the `utils/` directory with your API keys:

```env
CLAUDE_API_KEY="your_claude_api_key_here"
OPENAI_API_KEY="your_openai_api_key_here"
GEMINI_API_KEY="your_gemini_api_key_here"
```

**Getting API Keys:**

- **Claude**: Sign up at [Anthropic Console](https://console.anthropic.com/)
- **OpenAI**: Sign up at [OpenAI Platform](https://platform.openai.com/)
- **Gemini**: Sign up at [Google AI Studio](https://aistudio.google.com/)

## Usage

Open and run any of the demo notebooks:

- `main_claude_demo.ipynb` - Generate tongue-twisters with Claude
- `main_openai_demo.ipynb` - Create images from text with OpenAI
- `main_gemini_demo.ipynb` - Detect objects in images with Gemini

### Demo Examples

**Claude Demo:**

- Generates creative tongue-twisters on demand
- Compares zero-shot vs one-shot prompting results
- Example output: "Slippery snakes slither slowly through slimy, soggy swamps"

**OpenAI Demo:**

- Creates images from descriptive prompts
- Example: "A realistic Dalmatian pup at a birthday party"
- Saves high-quality images to the output directory

**Gemini Demo:**

- Detects objects in sample images
- Returns CSV with coordinates and confidence scores
- Creates annotated images with bounding boxes

## License

MIT License - Feel free to use this project for learning and experimentation.
