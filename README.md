# FractureNet: AI-Powered Medical Imaging Analysis

FractureNet is a revolutionary AI-powered medical imaging analysis platform designed to assist radiologists in detecting fractures instantly and accurately. Leveraging advanced deep learning technology, FractureNet analyzes X-ray images in seconds, providing precise fracture detection and detailed diagnostic insights.

## Features

- **Instant Fracture Detection**: AI models analyze X-ray images with clinical-grade precision (accuracy >90%).
- **Rapid Analysis**: Get results in less than 15 seconds.
- **Advanced AI**: Utilizes deep learning technology and convolutional neural networks specifically designed for medical imaging analysis.
- **Real-time Processing**: Provides instant analysis with detailed heatmaps and confidence scoring for immediate diagnosis.
- **Medical Grade Security**: HIPAA compliant infrastructure with end-to-end encryption for patient data protection.
- **Intuitive Dashboard**: User-friendly interface for uploading images, viewing analysis results, and tracking recent cases.
- **Dynamic Analytics**: Displays real-time total analyses count.

## Technologies Used

**Frontend:**
- Next.js
- React
- Tailwind CSS
- Framer Motion (for animations)

**Backend:**
- FastAPI
- PyTorch (for AI model)
- Uvicorn

## Setup and Installation

To set up FractureNet locally, follow these steps:

### 1. Clone the Repository

```bash
git clone https://github.com/ShaikhWarsi/FractureNet.git
cd FractureNet
```

### 2. Backend Setup

Navigate to the `backend` directory:

```bash
cd backend
```

Create a virtual environment and install dependencies:

```bash
python -m venv venv
venv\Scripts\activate  # On Windows
# source venv/bin/activate  # On macOS/Linux
pip install -r requirements.txt
```

Run the backend server:

```bash
uvicorn app:app --reload
```

The backend server will typically run on `http://localhost:8000`.

### 3. Frontend Setup

Open a new terminal and navigate to the `frontend` directory:

```bash
cd frontend
```

Install Node.js dependencies:

```bash
npm install
```

Run the frontend development server:

```bash
npm run dev
```

The frontend application will typically run on `http://localhost:3000` (or another available port like `3001`, `3002`, etc., if 3000 is in use).

## Usage

1. **Access the Application**: Open your web browser and navigate to the frontend URL (e.g., `http://localhost:3000`).
2. **Upload X-ray Image**: On the dashboard, use the upload zone to select and upload an X-ray image.
3. **View Analysis**: The AI will process the image, and the analysis results, including fracture detection, confidence scores, and heatmaps, will be displayed.
4. **Explore Features**: Navigate through the dashboard to view recent cases, system status, and other analytics.

## Project Structure

```
. \
├── backend/              # FastAPI backend for AI model inference and API endpoints
│   ├── Final.pt          # Pre-trained AI model
│   ├── analysis_count.json # Stores total analysis count
│   ├── app.py            # Main backend application
│   ├── results/          # Stores analysis results (GradCam, explanations)
│   └── uploads/          # Stores uploaded images
├── frontend/             # Next.js frontend application
│   ├── app/              # Next.js pages (dashboard, about, analytics, etc.)
│   ├── components/       # Reusable React components
│   ├── public/           # Static assets (images, icons)
│   └── ...               # Other Next.js configuration and files
└── requirements.txt      # Python dependencies for the backend
```

## Contributing

Contributions are welcome! Please feel free to fork the repository, create a new branch, and submit a pull request.

## License

This project is licensed under the MIT License.