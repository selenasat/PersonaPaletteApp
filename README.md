# Persona Palette App

A personal project to build a virtual style consultant that provides personalized fashion and beauty recommendations. This app uses computer vision to analyze a user's photos and determine their unique **color season**, **face shape**, and **body shape**.

## 🎨 Project Features
* **User Authentication:** Secure sign up, log in, and log out functionality.
* **Image Upload:** A user interface to securely upload photos for analysis.
* **Color Season Analysis:** Analyzes skin, hair, and eye tones to determine a user's core color season and detailed **sub-season** (e.g., Cool Winter, True Spring, Soft Summer).
* **Face Shape Analysis:** Classifies face shape and provides a list of recommended hairstyles and glasses.
* **Body Shape Analysis:** Determines body type and suggests flattering clothing silhouettes and styles.
* **Personalized Recommendations:** Delivers tailored advice based on all analysis results to help users curate a wardrobe that enhances their natural features.
* **Cross-Platform Compatibility:** A consistent experience across both a responsive website and a mobile application.
* **User Dashboard:** A personal space for users to view and manage their analyzed photos and saved recommendations.

## 🖌️ Design & Mockups
The user interface and user experience were designed and prototyped using **Figma**.

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
    git clone [https://github.com/selenasat/PersonaPaletteApp.git](https://github.com/selenasat/PersonaPaletteApp.git)
    cd PersonaPaletteApp
    ```

2.  **Set up environment variables:**
    * Create a `.env` file in the root of your project.
    * Add your sensitive information, such as `DATABASE_URL` and cloud storage keys, to this file.

3.  **Set up the backend (Django):**
    ```bash
    # Create a virtual environment
    python3 -m venv venv
    source venv/bin/activate
    # Install dependencies once you have a requirements.txt file
    pip install -r requirements.txt
    ```

4.  **Set up the database:**
    * Create a new PostgreSQL database.
    * Update the database settings in your `settings.py` file to reference your `.env` file.
    * Run database migrations:
    ```bash
    python manage.py makemigrations
    python manage.py migrate
    ```

5.  **Set up the frontend (React/React Native):**
    ```bash
    cd frontend-web # or frontend-mobile
    npm install
    ```

6.  **Run the application:**
    * Start the Django backend server:
    ```bash
    python manage.py runserver
    ```
    * Start the React development server:
    ```bash
    cd frontend-web
    npm start
    ```

## 📋 How to Use
Once the application is running, here is a general workflow:
1.  **Sign Up & Log In:** Create an account to access the dashboard.
2.  **Upload Photos:** Use the image upload interface to submit clear photos of your face and body.
3.  **View Analysis:** The app will process your photos and display a detailed analysis of your color season, face shape, and body type on your dashboard.
4.  **Explore Recommendations:** Browse personalized recommendations for colors, hairstyles, and clothing styles based on your results.

## 📸 Screenshots
[Add a screenshot of your app's user interface here, or a GIF showcasing its functionality.]

## 💡 Future Enhancements

* **Advanced Analysis & Technology**
    * Adding a feature to save analysis history and track style evolution.
    * Expanding the recommendations engine to include specific clothing items from popular brands.
    * Integrating a makeup recommendations module.
    * Integrating machine learning models for more precise image analysis.
    * Augmented Reality (AR) "Try-On" for recommended hairstyles, makeup, or accessories.
    * Seasonal trend integration to suggest ways to incorporate them into a user's style.
    * Advanced color matching by analyzing a photo of an item.

* **Community & Social Features**
    * Allowing users to create a profile and share their analyzed photos and favorite outfits.
    * An outfit planner to help users plan their weekly looks.
    * A gallery of community-sourced outfits, with filters based on body type, color season, and style.

* **Personalization & Business**
    * A virtual wardrobe feature for users to upload and manage photos of their own clothing.
    * A premium subscription tier to unlock exclusive features and content.

---

### License
This project is licensed under the MIT License - see the LICENSE.md file for details.
