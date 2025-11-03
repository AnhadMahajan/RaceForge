# RaceForge AI Flask Backend

This Flask backend service provides 3D model generation capabilities for the RaceForge AI project. It handles both text-to-3D and image-to-3D conversions using advanced AI models.

## Features

- Text to 3D model conversion
- Image to 3D model conversion
- API endpoints for model generation
- Shap-E model integration

## Project Structure

```
flaskk/
├── app.py              # Main Flask application
├── image_to_3d.py      # Image to 3D conversion logic
├── textto3d.py         # Text to 3D conversion logic
├── requirements.txt    # Python dependencies
├── outputs/           # Generated 3D models output directory
└── shap_e_model_cache/ # Pre-trained model files
```

## Setup

1. Create a virtual environment:
```bash
python -m venv env
source env/bin/activate  # On Windows: env\Scripts\activate
```

2. Install dependencies:
```bash
pip install -r requirements.txt
```

## Running the Server

Start the Flask server:
```bash
python app.py
```

The server will start on `http://localhost:5000` by default.

## API Endpoints

### Text to 3D
```
POST /api/text-to-3d
Content-Type: application/json

{
    "prompt": "your text description"
}
```

### Image to 3D
```
POST /api/image-to-3d
Content-Type: multipart/form-data

file: [image file]
```

## Dependencies

Key dependencies include:
- Flask
- PyTorch
- Shap-E
- CLIP

## Model Cache

The `shap_e_model_cache/` directory contains necessary pre-trained models for 3D generation:
- Image conditioning model
- Text conditioning model
- Transmitter model
- CLIP ViT-L-14 model

## Output Format

Generated 3D models are saved in the `outputs/` directory in compatible 3D file formats.

## Note

This backend is designed to work with the RaceForge AI frontend. Make sure both services are running for full functionality.