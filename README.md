# People-Count
## Overview
This project is a comprehensive People or person count system designed to monitor occupancy levels.
## Features
- **Dataset**: Utilizes a dataset of Yolov7.
- **Model**: Trained using YOLOv7, optimized with NVIDIA DGX A100 for accelerated processing.
- **Alert System**: Integrated with Gmail API via Google Cloud to notify users of non-compliance.
- **Real-time Detection**: Capable of detecting PPE in real-time from video feeds.
- **Containerization**: The entire project is containerized using Docker and deployed on an NVIDIA DGX A100.
- **Frontend**: A minimalist Flask frontend for easy monitoring of detection processes.

## Installation

### Prerequisites
- Docker
- NVIDIA Docker Toolkit
- Python 3.8+
- Flask
- YOLOv7 dependencies
- Google Cloud credentials for Gmail API

### Clone the Repository
```bash
git clone https://github.com/Harsha-108/PPE-Violation-Detection.git
cd PPE-Violation-Detection
```
### Install Python Dependencies
```bash
pip install -r requirements.txt
```
### Run the Application
```bash
python app.py
```
### Usage
- Real-time Detection
- Connect your video feed to the system.
- Access the Flask frontend at http://localhost:5000 to monitor detection in real-time.

### Alert System
- Ensure your Google Cloud credentials are properly set up to enable email notifications for non-compliance. The system will automatically send alerts to designated users.

### Acknowledgements
- Roboflow for the dataset curation tools.
- NVIDIA for providing the DGX A100.
- Google Cloud for the Gmail API.
