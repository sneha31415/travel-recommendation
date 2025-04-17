# Travel Recommendation System

A Flask-based web application that provides personalized travel recommendations using machine learning models.

## Features

- Collaborative filtering for destination recommendations
- Popularity prediction for destinations
- User-friendly web interface
- Personalized recommendations based on user preferences

## Prerequisites

- Python 3.x
- Flask
- Pandas
- scikit-learn
- NumPy

## Installation

1. Clone the repository:
```bash
git clone <repository-url>
cd travel-recommendation
```

2. Create and activate a virtual environment:
```bash
# On Windows
python -m venv venv
venv\Scripts\activate

# On macOS/Linux
python3 -m venv venv
source venv/bin/activate
```

3. Install required packages:
```bash
pip install flask pandas scikit-learn numpy
```

4. Deactivate the virtual environment when done:
```bash
deactivate
```

## Running the Application

1. Activate the virtual environment:
```bash
# On Windows
venv\Scripts\activate

# On macOS/Linux
source venv/bin/activate
```

2. Start the Flask server:
```bash
python app.py
```

3. Open your web browser and navigate to:
```
http://127.0.0.1:5000/recommendations
```

4. When you're done, deactivate the virtual environment:
```bash
deactivate
```

## How to Use

1. Enter your User ID (must be a valid ID from the dataset)
2. Fill in the following details:
   - Destination Name
   - Type of destination
   - State
   - Best Time to Visit
   - Preferences
   - Gender
   - Number of Adults
   - Number of Children

3. Click "Get Recommendations" to receive personalized travel suggestions

## Project Structure

- `app.py` - Main Flask application
- `templates/` - HTML templates
  - `recommendations.html` - Main recommendation form
- `code and dataset/` - Contains the ML models and datasets
  - `model.pkl` - Trained ML model
  - `label_encoders.pkl` - Label encoders for categorical data
  - `Expanded_Destinations.csv` - Destination dataset
  - `Final_Updated_Expanded_UserHistory.csv` - User history dataset
  - `final_df.csv` - Final processed dataset
- `venv/` - Virtual environment directory (created during setup)

## Note

The application uses pre-trained models and datasets. Make sure all the required files are present in the `code and dataset/` directory before running the application.

## Virtual Environment Benefits

Using a virtual environment:
- Isolates project dependencies
- Prevents conflicts between different projects
- Makes it easier to manage package versions
- Ensures reproducibility across different machines
- Keeps your global Python installation clean 