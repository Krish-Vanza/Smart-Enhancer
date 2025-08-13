# AI Image Enhancer

A modern web application to enhance images using an AI-powered API. Users can upload images, preview the original and enhanced versions, and download the enhanced result. The app enforces strict validation for file type, size, and dimensions.

## Features
- Upload images (PNG, JPG, JPEG, WEBP, GIF, BMP, TIFF)
- File validation: max 15MB, max 4096x4096 pixels
- Preview original and enhanced images side by side
- Download enhanced images
- Responsive, clean UI with Tailwind CSS
- Asynchronous enhancement with loading indicator

## Getting Started

### Prerequisites
- Node.js (v16 or higher recommended)
- npm or yarn

### Installation
1. Clone the repository:
   ```sh
   git clone <your-repo-url>
   cd AI-Image-Enhancer
   ```
2. Install dependencies:
   ```sh
   npm install
   # or
   yarn install
   ```
3. Create a `.env` file in the root directory and add your API credentials:
   ```env
   VITE_API_KEY=your_api_key_here
   VITE_BASE_URL=https://your-api-base-url.com
   VITE_MAXIMUM_RETRIES=10
   ```

### Running the App
```sh
npm run dev
# or
yarn dev
```
The app will be available at `http://localhost:5173` (or the port shown in your terminal).

## Project Structure
```
AI Image Enhancer/
├── src/
│   ├── components/
│   │   ├── Home.jsx
│   │   ├── ImagePreview.jsx
│   │   ├── ImageUpload.jsx
│   │   └── Loading.jsx
│   ├── utils/
│   │   └── enhanceImageAPI.js
│   ├── App.jsx
│   ├── App.css
│   ├── index.css
│   └── main.jsx
├── index.html
├── package.json
├── tailwind.config.js
├── postcss.config.js
├── vite.config.js
└── README.md
```

## Image Requirements
- **Maximum file size:** 15MB
- **Maximum dimensions:** 4096×4096 pixels
- **Supported formats:** PNG, JPG, JPEG, WEBP, GIF, BMP, TIFF

## Environment Variables
| Variable              | Description                |
|-----------------------|----------------------------|
| VITE_API_KEY          | Your API key               |
| VITE_BASE_URL         | API base URL               |
| VITE_MAXIMUM_RETRIES  | Max polling retries        |

## License
MIT
