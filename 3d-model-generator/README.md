# 3D Model Generator

A Next.js application for generating and viewing 3D models using AI technology.

## Features

- AI-powered 3D model generation
- Real-time 3D model viewing
- Image upload capabilities
- Responsive design
- Theme support
- Progress tracking
- Download capabilities

## Tech Stack

- **Framework**: Next.js 14
- **Language**: TypeScript
- **Styling**: Tailwind CSS
- **UI Components**: Shadcn/ui
- **3D Rendering**: Three.js
- **State Management**: React Hooks

## Getting Started

### Prerequisites

- Node.js (v18 or higher)
- pnpm

### Installation

```bash
# Install dependencies
pnpm install

# Start development server
pnpm dev
```

The application will be available at `http://localhost:3000`

## Project Structure

```
3d-model-generator/
├── app/                    # Next.js app directory
├── components/            # React components
├── hooks/                # Custom React hooks
├── lib/                  # Utility functions and services
├── public/              # Static assets
└── styles/              # Global styles
```

## API Endpoints

- `/api/rodin` - AI model generation endpoint
- `/api/download` - Model download endpoint
- `/api/status` - Generation status checking
- `/api/proxy-download` - Proxy for downloading models

## Component Usage

### Model Viewer

```tsx
import { ModelViewer } from '@/components/model-viewer'

<ModelViewer modelUrl="path/to/model" />
```

### Image Upload

```tsx
import { ImageUploadArea } from '@/components/image-upload-area'

<ImageUploadArea onUpload={(file) => handleUpload(file)} />
```

## Development

```bash
# Run tests
pnpm test

# Build for production
pnpm build

# Start production server
pnpm start
```

## Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit changes (`git commit -m 'Add amazing feature'`)
4. Push to branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## License

This project is licensed under the MIT License - see the LICENSE file for details.