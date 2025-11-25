# RaceForge-AI

RaceForge-AI is an innovative project that combines AI-powered 3D model generation with an interactive racing game experience. The project allows users to create custom 3D car models using AI and then use them in a racing game environment.  

## 🚀 Features

- AI-powered 3D model generation from text descriptions or images
- Interactive 3D model viewer
- Real-time racing game environment
- Custom car model integration
- Responsive web interface
- Server-side model processing

## 🏗️ Project Structure

The project consists of four main components:

1. **3D Model Generator** (Next.js Frontend)
   - AI-powered 3D model generation interface
   - Real-time model preview
   - User input handling for text and image uploads

2. **Flask Backend**
   - Handles AI model processing
   - Converts text/images to 3D models
   - Uses ShapeE AI models

3. **Main Frontend** (Vite + React)
   - User interface for the main application
   - Model management and preview
   - Game integration interface

4. **Racing Game** (Three.js)
   - 3D racing environment
   - Physics engine integration
   - Custom car model support

## 🛠️ Tech Stack

- **Frontend**: React, Next.js, Three.js, TypeScript
- **Backend**: Flask, Node.js, Express
- **AI Models**: ShapeE
- **3D Graphics**: Three.js
- **Styling**: Tailwind CSS
- **Build Tools**: Vite, Node.js

## 📋 Prerequisites

- Node.js 18.x or higher
- Python 3.8 or higher
- CUDA-compatible GPU (recommended for AI model processing)

## 🚀 Getting Started

1. Clone the repository:
```bash
git clone https://github.com/yourusername/RaceForge-AI.git
cd RaceForge-AI
```

2. Set up the Flask backend:
```bash
cd flaskk
python -m venv env
source env/bin/activate  # On Windows: .\env\Scripts\activate
pip install -r requirements.txt
python app.py
```

3. Set up the 3D model generator:
```bash
cd ../3d-model-generator
npm install
npm run dev
```

4. Set up the main frontend:
```bash
cd ../Frontend
npm install
npm run dev
```

5. Set up the racing game:
```bash
cd ../racing-game
npm install
npm run dev
```

## 💻 Usage

1. Access the 3D model generator at `http://localhost:3000`
2. Create your custom car model using text descriptions or image uploads
3. Preview and adjust the generated 3D model
4. Save your model and launch the racing game
5. Use your custom car in the racing environment

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## 📝 License

This project is licensed under the MIT License - see the LICENSE file for details.

## 🙏 Acknowledgments

- ShapeE AI model for 3D generation
- Three.js community
- React and Next.js teams

## 📞 Contact

For questions and support, please open an issue in the GitHub repository.
