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
Install Required Dependencies 
Install the necessary libraries manually. 
1. Open a terminal or command prompt 
2. Run the following command to install common dependencies:  
pip install flask tensorflow numpy pandas librosa scikit-learn  
If you encounter an error while running the project, check the missing module in the error      
message and install it using pip install <module_name>. 
Step 3: Run the Jupyter Notebooks 
The main code is inside speech-emotion-recognizer-movie-recommendation.ipynb and 
flask1.ipynb. 
1. Open a terminal and navigate to the project folder:  
cd path/to/project-folder 
2. Start Jupyter Notebook:  
jupyter notebook 
3. Open and Run the following notebooks in order:  
a. speech-emotion-recognizer-movie-recommendation.ipynb (Main model 
execution) 
b. flask1.ipynb (Flask API for local hosting) 
Step 4: Start the Flask Web App 
If the Flask server is not already running via the notebook, you might need to manually start it. 
1. Navigate to the folder where Flask is set up. 
2. If you want to run the Flask server without Jupyter Notebook, do this: 
3. Convert the notebook to a Python script  
jupyter nbconvert --to script flask1.ipynb 
4. This will generate a file called flask1.py. 
5. Rename it to app.py  
mv flask1.py app.py   # On Linux/Mac 
ren flask1.py app.py  # On Windows 
6. Run Flask manually:  
python app.py 
7. Open your browser and go to: 
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
File Structure 
SPEECH-Emotion-Based-Movie-Recommender-System 
├── flask1.ipynb 
                # Flask server for web app 
├── speech-emotion-recognizer-movie-recommendation.ipynb  # Main Model Code 
├── model.json 
                   # Trained Model Architecture 
├── features.csv                   # Extracted Features from Speech 
├── prototype.html
                 # Web Page HTML 
├── look.css 
                      # Web Page CSS 
