# AI Document Intelligence & Automation System

## 📋 Description

A comprehensive end-to-end document processing system that leverages Artificial Intelligence to automatically extract, classify, and analyze information from documents. This solution combines OCR (Optical Character Recognition), Document Classification, Named Entity Recognition (NER), and Automated Data Extraction into a single powerful pipeline.

## 🎯 What This System Does

This system transforms unstructured documents (PDFs, images, scanned files) into structured, actionable data through a multi-stage AI pipeline:

1. **📄 OCR Processing**: Converts images and PDFs to machine-readable text using Tesseract OCR
2. **🏷️ Document Classification**: Automatically categorizes documents (Invoices, Contracts, ID Proofs, etc.)
3. **🔍 Named Entity Recognition**: Identifies and extracts key entities (Names, Dates, Amounts, IDs, etc.)
4. **📊 Data Extraction**: Structures extracted information into organized, queryable formats

## 💼 Industry Applications

### 🏦 Banking
- KYC Document Verification
- Loan Application Processing
- Account Opening Automation
- Financial Statement Analysis

### 🏥 Insurance
- Claim Form Processing
- Policy Document Analysis
- Risk Assessment Automation
- Medical Records Digitization

### 📦 Logistics
- Invoice Processing
- Shipping Label Recognition
- Waybill Analysis
- Supply Chain Documentation

## 🚀 Key Features

- **Zero to Hero Setup**: Complete from-scratch implementation
- **Attractive UI**: Modern, responsive React interface
- **AI-Powered**: Google Gemini API integration
- **Multiple Document Types**: Support for PDF, JPG, PNG, TIFF
- **Real-time Processing**: Instant results with visual feedback
- **Export Capabilities**: CSV, JSON, Excel exports
- **Processing History**: Track all document operations
- **Confidence Scoring**: See AI prediction reliability

## 🛠️ Technology Stack

### Frontend
- React 18 + Tailwind CSS
- Framer Motion for animations
- Chart.js for analytics
- Axios for API communication
- React Dropzone for file uploads

### Backend
- Python 3.9+ / FastAPI
- SQLAlchemy ORM
- PyTesseract OCR
- SpaCy NER
- Google Gemini AI
- OpenCV for image processing

### Database
- PostgreSQL (Production)
- SQLite (Development)

## 📁 Project Structure

## 🎨 UI Preview

The application features:
- **Dashboard**: Overview with statistics and charts
- **OCR Upload**: Drag-and-drop interface with preview
- **Classification View**: Auto-categorized documents
- **NER Analysis**: Highlighted entities with confidence scores
- **Extraction Table**: Structured data with export options

## 🚦 Quick Start

### Prerequisites
- Python 3.9+
- Node.js 16+
- Tesseract OCR
- PostgreSQL (optional)

### Backend Setup
```bash
# Clone repository
git clone https://github.com/yourusername/doc-intelligence-ai-system.git
cd doc-intelligence-ai-system

# Create virtual environment
python -m venv venv
source venv/bin/activate  # Windows: venv\Scripts\activate

# Install dependencies
pip install -r backend/requirements.txt

# Setup environment variables
cp .env.example .env
# Edit .env with your configuration

# Run backend server
uvicorn app.main:app --reload --host 0.0.0.0 --port 8000

# Navigate to frontend
cd frontend

# Install dependencies
npm install

# Start development server
npm start

# Build for production
npm run build