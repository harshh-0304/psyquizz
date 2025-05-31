# Psyche-Quiz 🧠
#### A Mental Health Monitoring Website

---

**Psyche-Quiz** is an open source webapp dedicated for testing depression. **Psyche-Quiz** allows people to test depression on this webapp, which are then predicted by a machine-learning algorithm. In **Psyche-Quiz** we help people to overcome their depression so that they can live in peace.

---

## Features ✨

- Interactive psychological quiz with real-time result prediction ! 
- Machine learning-powered mental health assessment using SVM !
- Automatic logging of user responses and results into CSV !
- Self-improving model trained on over 16,000 quiz sessions ! 
- Deployed and live on [Render](https://psyche-quiz.onrender.com/) for public use ! 
- Lightweight UI built using HTML, CSS, JavaScript, and Flask !

---

## Tech Stack 🛠️

| Layer        | Technology       |
|--------------|------------------|
| **Frontend** | HTML5, CSS3, JavaScript |
| **Backend**  | Python (Flask)   |
| **Machine Learning** | scikit-learn (SVM Classifier) |
| **Deployment**  | [Render](https://psyche-quiz.onrender.com/) |

---

## Algorithm 💡

The core of the Psyche Quiz's prediction engine is a **Support Vector Machine (SVM)** classifier. Based on responses to 10 psychological questions, the SVM predicts one of several mental health labels. SVM was chosen for its balance of accuracy, speed, and interpretability in high-dimensional feature spaces - a great fit for lightweight mental health analysis.

---

## Data Handling 📊

Every time a user completes the quiz, their answers and predicted result are stored in a CSV file. This dataset is then used to incrementally retrain the model, allowing it to improve over time. Currently, the system has processed and learned from **16,000+ quiz entries**, making it more personalized and accurate as it grows.

---

## Project Structure 📁

| File/Folder       | Description                                            |
|-------------------|--------------------------------------------------------|
| `dataset/`        | Stores `data.csv` file with cumulative quiz results    |
| `static/`         | Contains CSS, JS, and static frontend assets           |
| `templates/`      | HTML templates for rendering pages via Flask           |
| `Procfile`        | Specifies process type for deployment on Render        |
| `README.md`       | Project documentation (you’re reading it!)             |
| `models.py`       | Contains SVM model logic for prediction & retraining   |
| `requirements.txt`| Python dependencies needed to run the project          |
| `server.py`       | Main Flask application and routing logic               |

---

## Installation & Setup Instructions ⚙️

To run the project locally, follow these steps:
1. **Clone the Repository or Download zip**
2. **Create Virtual Environment (Recommended)**
   ```bash
   python -m venv venv
   venv\Scripts\activate
   ```
3. **Install Dependencies**
   ```bash
   pip install -r requirements.txt
   ```
4. **Run the Application**
   ```bash
   python server.py
   ```
5. **Access the App in your Browser**
   ```bash
   http://localhost:5000
   ```

✔️ **Deployed Version** The Project is hosted on **Render**. - https://psyche-quiz.onrender.com/

---

## Author/Credits 👥

This project was developed by a team of four passionate developers as part of a collaborative initiative to explore machine learning applications in mental health:

- **Mayin Machhoya** 
- **Harsh Patel** 
- **Harsh Jadav** 
- **Shashank Mengar**

Special thanks to all contributors, testers, and early users who helped improve the project through their valuable feedback.

> 🧠 Built with care to help minds, one quiz at a time.
