# Persona Palette App

A personal project to build a virtual style consultant that provides personalized fashion and beauty recommendations. This app uses computer vision to analyze a user's photos and determine their unique **color season**, **face shape**, and **body shape**.

## 🎨 Features
* **Color Season Analysis:** Analyzes skin, hair, and eye tones to determine a user's color palette (e.g., Spring, Summer, Autumn, Winter).
* **Face Shape Analysis:** Identifies key facial landmarks to classify a user's face shape (e.g., Oval, Round, Square) and provide a list of recommended hairstyles and accessories.
* **Body Shape Analysis:** Measures body proportions to determine a user's body type (e.g., Hourglass, Pear, Apple) and suggests flattering clothing silhouettes.
* **Personalized Recommendations:** Delivers tailored advice based on the analysis results to help users curate a wardrobe that enhances their natural features.

## 🚀 Tech Stack
* **Backend:** Python with the Django framework
* **Data Analysis:** Python libraries including **OpenCV** and **Pillow**
* **Database:** **PostgreSQL**
* **Frontend (Web):** **React**
* **Frontend (Mobile):** **React Native**
* **Cloud Storage:** [**AWS S3 / Google Cloud Storage**] for image hosting

## 💻 Getting Started
These instructions will help you set up the project locally for development and testing.

### Prerequisites

You will need the following installed on your machine:
* Python 3.x
* Node.js and npm/yarn
* PostgreSQL

### Installation

1.  **Clone the repository:**
    ```bash
    git clone [your-repository-url]
    cd [your-repository-name]
    ```

2.  **Set up the backend (Django):**
    ```bash
    # Create a virtual environment
    python3 -m venv venv
    source venv/bin/activate
    # Install dependencies
    pip install -r requirements.txt
    ```

3.  **Set up the database:**
    * Create a new PostgreSQL database.
    * Update the database settings in your `settings.py` file.
    * Run database migrations:
    ```bash
    python manage.py makemigrations
    python manage.py migrate
    ```

4.  **Set up the frontend (React/React Native):**
    ```bash
    cd frontend-web # or frontend-mobile
    npm install
    ```

5.  **Run the application:**
    * Start the Django backend server:
    ```bash
    python manage.py runserver
    ```
    * Start the React development server:
    ```bash
    cd frontend-web
    npm start
    ```

## 📸 Screenshots
[Add a screenshot of your app's user interface here, or a GIF showcasing its functionality.]

## 💡 Future Enhancements
* Adding a feature to save analysis history and track style evolution.
* Expanding the recommendations engine to include specific clothing items from popular brands.
* Integrating machine learning models for more precise image analysis.

---

### License
This project is licensed under the MIT License - see the LICENSE.md file for details.