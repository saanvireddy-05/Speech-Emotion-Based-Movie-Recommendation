# Speech-Emotion-Based-Movie-Recommendation
README- 
Emotion-Based Movie Recommender System 
Overview 
This project is an Emotion-Based Movie Recommendation System that analyzes speech input 
to detect emotions and suggests movies accordingly. It utilizes Convolutional Neural Networks 
(CNNs) for speech emotion recognition and a prediction model to recommend movies based on 
the identified emotion. 
Features 
• Speech Emotion Recognition: Uses MFCC, Chroma, and Mel features to analyze 
input speech. 
• CNN Model for Emotion Detection: Classifies emotions from speech input. 
• Movie Recommendation System: Suggests movies based on detected emotions. 
• Web Interface: Built using HTML, CSS, and Flask for user interaction. 
How To Run? 
### Step 1: Install Required Dependencies 
### Step 2: Install the necessary libraries manually. 
1. Open a terminal or command prompt 
2. Run the following command to install common dependencies:
``` bash  
pip install flask tensorflow numpy pandas librosa scikit-learn
```
If you encounter an error while running the project, check the missing module in the error      
message and install it using ``` bash pip install <module_name>``` 
### Step 3: Run the Jupyter Notebooks 
The main code is inside speech-emotion-recognizer-movie-recommendation.ipynb and 
flask1.ipynb. 
1. Open a terminal and navigate to the project folder:  
``` bash
cd path/to/project-folder
```
2. Start Jupyter Notebook:
``` bash
jupyter notebook
``` 
4. Open and Run the following notebooks in order:  
a. speech-emotion-recognizer-movie-recommendation.ipynb (Main model 
execution) 
b. flask1.ipynb (Flask API for local hosting) 
### Step 4: Start the Flask Web App 
If the Flask server is not already running via the notebook, you might need to manually start it. 
1. Navigate to the folder where Flask is set up. 
2. If you want to run the Flask server without Jupyter Notebook, do this: 
3. Convert the notebook to a Python script
``` bash 
jupyter nbconvert --to script flask1.ipynb
```
5. This will generate a file called flask1.py. 
6. Rename it to app.py
``` bash
mv flask1.py app.py   # On Linux/Mac 
ren flask1.py app.py  # On Windows
```
8. Run Flask manually:
9.Or by using
``` bash
python app.py
```
10. Open your browser and go to: 
http://127.0.0.1:5000/ 
Step 5: Test the Emotion-Based Movie Recommender 
1. Upload an audio file (speech sample). 
2. The system will analyze the emotion. 
3. It will recommend movies based on the detected emotion. 
Dataset Setup 
• As the project  requires the RAVDESS Dataset, you may need to download it manually:  
o Download RAVDESS Dataset 
o Extract and place it in the correct folder as referenced in the code. 
o Update the dataset path in the notebook or Flask app if needed. 
Link for Trained Model: 
https://drive.google.com/file/d/1Ka5RIAwvkVDy3qWR5V8QTmbOOsjhHOhT/view?usp=sharing 
DEMO VIDEO                       
https://drive.google.com/file/d/1B8wypc7OWDciAkM6gANHpNdKxuYOGbta/view?usp=sharing

```
SPEECH-Emotion-Based-Movie-Recommender-System
├── flask1.ipynb                          # Flask server for web app
├── speech-emotion-recognizer-movie-recommendation.ipynb  # Main model code
├── model.json                           # Trained model architecture
├── features.csv                         # Extracted features from speech
├── prototype.html                       # Web page HTML
├── look.css                             # Web page CSS
```

