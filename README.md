🩺 Disease Prediction System using Machine Learning & Flask
### Code Requirements
Python Version > 3.5

A web-based Disease Prediction Application built using Machine Learning (Decision Tree Classifier), Python, Flask, and Google Geolocation API.
Users can select symptoms from a dropdown and instantly get a predicted disease along with the option to find the nearest hospital using Google Maps.

🚀 Features
🔍 1. Disease Prediction
ML model trained on Training.csv
Uses Decision Tree Classifier
Users select up to 5 symptoms
System returns the most likely disease

🏥 2. Nearest Hospital Finder (Google Geolocation API)
User enters a location
App displays the nearest hospitals from Google Maps

🎨 3. Web UI (Flask + HTML/CSS)
Dropdown to select symptoms
Disease result page
Hospital location page

🧠 Machine Learning Model
📁 Dataset
Training.csv → Used to train the model
Testing.csv → Used to load symptoms list for dropdown

🧾 Algorithm Used
DecisionTreeClassifier (scikit-learn)
Multi-class classification
Predicts disease based on one-hot encoded symptoms

🧩 Input Format
The ML model expects 132 symptoms, represented as a binary vector (0/1).
Example:
['headache', 'muscle_weakness']

🔍 Prediction Function
def dosomething(symptom):
    user_input_label = [0 for i in range(132)]
    for i in symptom:
        idx = dictionary[i]
        user_input_label[idx] = 1
    return dt.predict([user_input_label])

⚙️ Installation & Setup
1. Clone the Repository
git clone https://github.com/bot041/Virtual-Health-Assistance-Using-Machine-Learning-And-Flask.git
cd Disease-Prediction-system-using-Machine-Learning-and-Flask

2. Install Dependencies
Make sure Python 3.x is installed.
pip install -r requirements.txt
If requirements.txt is not present, install manually:
pip install flask pandas numpy scikit-learn

3. Run the Application
python app.py
App runs at:
http://127.0.0.1:5000/

🖥️ How It Works (User Flow)

🏁 Step 1 — Home Page
User sees symptom dropdowns:
Symptom1,
Symptom2,
Symptom3,
Symptom4,
Symptom5.

🔮 Step 2 — Predict Disease
User selects symptoms → Clicks Predict →
App returns:
Disease Name
Suggested treatment/medicines (if implemented)

🗺️ Step 3 — Find Nearest Hospital
User enters location → App loads:
Google Maps with nearest hospitals
Interactive map

🔑 APIs Used
✔ Google Maps Geolocation API
Used to find nearby hospitals:
Requires API Key
Can be added in find_doctor.html

📌 Important Files

🔹 diseaseprediction.py
Handles:
Dataset loading
ML model training
Prediction logic

🔹 app.py
Handles:
Flask routes
HTML rendering
Connecting ML model with UI

💡 Future Enhancements
Add medicine recommendations
Add disease descriptions
Improve UI with Bootstrap / Tailwind
Add user login system
Store prediction history in a database.

👨‍💻 Author

Bhuvan Kambad

Email: bkambad041@gmail.com

