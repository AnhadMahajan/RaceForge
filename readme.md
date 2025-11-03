# RaceForge-AI

Monorepo containing the RaceForge-AI frontend, Python services, and 3D model tools.

## Contents

- [3d-model-generator](3d-model-generator/) — Next.js 3D model generation UI and utilities. See [3d-model-generator/README.md](3d-model-generator/README.md).
- [Frontend](Frontend/) — Main web frontend (Vite + React + TypeScript).
  - Frontend entry: [Frontend/package.json](Frontend/package.json)
  - Frontend app root: [Frontend/src/main.tsx](Frontend/src/main.tsx)
  - Example page for model generation: [Frontend/src/pages/generatemodel.tsx](Frontend/src/pages/generatemodel.tsx)
  - Example 3D component: [Frontend/src/components/CarModel.tsx](Frontend/src/components/CarModel.tsx)
  - Backend server (in repo frontend/backend): [Frontend/backend/server.js](Frontend/backend/server.js)
- [flaskk](flaskk/) — Python Flask utilities and scripts for converting images/text to 3D.
  - Flask app: [flaskk/app.py](flaskk/app.py)
  - Image-to-3D script: [flaskk/image_to_3d.py](flaskk/image_to_3d.py)
  - Text-to-3D script: [flaskk/textto3d.py](flaskk/textto3d.py)
- [racing-game](racing-game/) — (game project folder)

## Quickstart

Prereqs:
- Node 18+ (or Bun if you use bun.lockb) for frontend
- Python 3.8+ and virtualenv for Flask services
- pnpm / npm as preferred package manager

Frontend:
1. cd Frontend
2. Install: `npm install` (or `pnpm install` / `bun install`)
3. Start dev server: `npm run dev`
4. Backend mock server: cd Frontend/backend && `npm install` && `node server.js` (see [Frontend/backend/server.js](Frontend/backend/server.js))

Flask services:
1. cd flaskk
2. Create venv: `python -m venv env && source env/bin/activate` (Windows: `env\Scripts\activate`)
3. Install deps: `pip install -r requirements.txt`
4. Run: `python app.py` (exposes Flask API — see [flaskk/app.py](flaskk/app.py))
5. Scripts: [flaskk/image_to_3d.py](flaskk/image_to_3d.py) and [flaskk/textto3d.py](flaskk/textto3d.py) are utilities used by the service.

3D Model Generator (Next.js):
1. cd 3d-model-generator
2. Install: `npm install`
3. Dev: `npm run dev`
4. See [3d-model-generator/README.md](3d-model-generator/README.md) for details.

## Project layout (high level)
- 3d-model-generator/ — Next.js + 3D utilities
- Frontend/ — Vite React app + a simple backend
  - [Frontend/src/pages/generatemodel.tsx](Frontend/src/pages/generatemodel.tsx)
  - [Frontend/src/components/CarModel.tsx](Frontend/src/components/CarModel.tsx)
- flaskk/ — Flask app & helper scripts
  - [flaskk/app.py](flaskk/app.py)
  - [flaskk/image_to_3d.py](flaskk/image_to_3d.py)
  - [flaskk/textto3d.py](flaskk/textto3d.py)

## Notes
- Use the example pages and components in [Frontend/src/](Frontend/src/) to see how the frontend integrates with the backend.
- For seeding sample data, check [Frontend/backend/scripts/seedCars.js](Frontend/backend/scripts/seedCars.js).
- Adjust environment variables in [Frontend/.env](Frontend/.env) and [Frontend/backend/.env](Frontend/backend/.env).

If you want, I can:
- generate README sections per subproject,
- add run/debug launch configs for VS Code,
- or create a CONTRIBUTING.md.

```// filepath: README.md
# RaceForge-AI

Monorepo containing the RaceForge-AI frontend, Python services, and 3D model tools.

## Contents

- [3d-model-generator](3d-model-generator/) — Next.js 3D model generation UI and utilities. See [3d-model-generator/README.md](3d-model-generator/README.md).
- [Frontend](Frontend/) — Main web frontend (Vite + React + TypeScript).
  - Frontend entry: [Frontend/package.json](Frontend/package.json)
  - Frontend app root: [Frontend/src/main.tsx](Frontend/src/main.tsx)
  - Example page for model generation: [Frontend/src/pages/generatemodel.tsx](Frontend/src/pages/generatemodel.tsx)
  - Example 3D component: [Frontend/src/components/CarModel.tsx](Frontend/src/components/CarModel.tsx)
  - Backend server (in repo frontend/backend): [Frontend/backend/server.js](Frontend/backend/server.js)
- [flaskk](flaskk/) — Python Flask utilities and scripts for converting images/text to 3D.
  - Flask app: [flaskk/app.py](flaskk/app.py)
  - Image-to-3D script: [flaskk/image_to_3d.py](flaskk/image_to_3d.py)
  - Text-to-3D script: [flaskk/textto3d.py](flaskk/textto3d.py)
- [racing-game](racing-game/) — (game project folder)

## Quickstart

Prereqs:
- Node 18+ (or Bun if you use bun.lockb) for frontend
- Python 3.8+ and virtualenv for Flask services
- pnpm / npm as preferred package manager

Frontend:
1. cd Frontend
2. Install: `npm install` (or `pnpm install` / `bun install`)
3. Start dev server: `npm run dev`
4. Backend mock server: cd Frontend/backend && `npm install` && `node server.js` (see [Frontend/backend/server.js](Frontend/backend/server.js))

Flask services:
1. cd flaskk
2. Create venv: `python -m venv env && source env/bin/activate` (Windows: `env\Scripts\activate`)
3. Install deps: `pip install -r requirements.txt`
4. Run: `python app.py` (exposes Flask API — see [flaskk/app.py](flaskk/app.py))
5. Scripts: [flaskk/image_to_3d.py](flaskk/image_to_3d.py) and [flaskk/textto3d.py](flaskk/textto3d.py) are utilities used by the service.

3D Model Generator (Next.js):
1. cd 3d-model-generator
2. Install: `npm install`
3. Dev: `npm run dev`
4. See [3d-model-generator/README.md](3d-model-generator/README.md) for details.

## Project layout (high level)
- 3d-model-generator/ — Next.js + 3D utilities
- Frontend/ — Vite React app + a simple backend
  - [Frontend/src/pages/generatemodel.tsx](Frontend/src/pages/generatemodel.tsx)
  - [Frontend/src/components/CarModel.tsx](Frontend/src/components/CarModel.tsx)
- flaskk/ — Flask app & helper scripts
  - [flaskk/app.py](flaskk/app.py)
  - [flaskk/image_to_3d.py](flaskk/image_to_3d.py)
  - [flaskk/textto3d.py](flaskk/textto3d.py)

