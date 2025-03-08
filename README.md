# Personalized-Medical-Recommendation-System-with-Machine-Learning
## Disease Prediction and Medicine Recommendation System

## Overview
This project is a Flask-based web application that predicts diseases based on user-provided symptoms and recommends appropriate medications, precautions, and diet plans. It leverages a trained Support Vector Classifier (SVC) model to classify diseases and provides additional health recommendations.

## Features
- Predict diseases based on user input symptoms.
- Recommend medications for predicted diseases.
- Provide precautions and dietary suggestions.
- Suggest workouts for specific diseases.
- User-friendly web interface for interaction.

## Technologies Used
- **Python** (Flask, NumPy, Pandas, Pickle)
- **Machine Learning** (Support Vector Classifier - SVC)
- **Frontend** (HTML, CSS, JavaScript - rendered through Flask templates)
- **Dataset** (CSV files for symptoms, descriptions, precautions, medications, and diet plans)

## Installation & Setup

1. **Clone the Repository:**
   ```bash
   git clone https://github.com/your-repo/disease-prediction.git
   cd disease-prediction
   ```

2. **Create a Virtual Environment (Optional but Recommended):**
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. **Install Dependencies:**
   ```bash
   pip install -r requirements.txt
   ```

4. **Run the Application:**
   ```bash
   python app.py
   ```

5. **Access the Application:**
   Open your browser and go to `http://127.0.0.1:5000/`

## Project Structure
```
├── datasets/
│   ├── symptoms_df.csv
│   ├── precautions_df.csv
│   ├── workout_df.csv
│   ├── description.csv
│   ├── medications.csv
│   ├── diets.csv
│
├── models/
│   ├── svc.pkl  # Trained ML model for disease prediction
│
├── templates/
│   ├── index.html  # Main UI template
│   ├── about.html  # About page
│   ├── contact.html  # Contact page
│   ├── developer.html  # Developer info page
│   ├── blog.html  # Blog page
│
├── app.py  # Flask application
├── requirements.txt  # Dependencies
├── README.md  # Project documentation
```

## API Routes

| Route         | Method | Description |
|--------------|--------|-------------|
| `/`          | GET    | Home page |
| `/predict`   | POST   | Predicts disease based on symptoms |
| `/about`     | GET    | About the project |
| `/contact`   | GET    | Contact page |
| `/developer` | GET    | Developer details |
| `/blog`      | GET    | Blog section |

## Usage
1. Enter symptoms in the input field, separated by commas.
2. Click on the **Predict** button.
3. The application will display:
   - Predicted disease name
   - Disease description
   - Recommended medications
   - Precautions to take
   - Suggested diet and workout plans

## Future Enhancements
- **Expand dataset** for more diseases and medications.
- **Improve ML model** with better training and fine-tuning.
- **Integrate API services** for real-time medical suggestions.
- **Enhance UI/UX** for a more interactive experience.

