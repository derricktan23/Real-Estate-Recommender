# Real Estate Recommender System
![Architecture Diagram](https://github.com/user-attachments/assets/609d57c1-6ed8-43b6-ba21-8d1d73555b6e)

## Overview
The Real Estate Recommender System is a web application designed to help users find suitable properties based on their preferences. The system utilizes a hybrid recommendation approach, combining content-based and collaborative filtering methods to provide personalized property suggestions.

## Features
- **User Authentication**: Users can register and log in to access personalized features.
- **Property Upload**: Users can upload property data in CSV format to populate the database.
- **Recommendations**: The application provides tailored property recommendations based on user preferences and feedback.
- **Feedback System**: Users can give feedback on properties to improve future recommendations.

## Architecture
The application is built using a Flask backend and a Streamlit frontend, with an SQLite database for data storage. The architecture consists of:

- **Frontend (Streamlit)**: User interface for registration, login, file uploads, and viewing recommendations.
- **Backend (Flask API)**: Handles user requests, manages data processing, and interacts with the database.
- **Database (SQLite)**: Stores user information, property details, and user feedback.

## Technologies Used
- **Backend**: Flask, Flask-SQLAlchemy, Flask-Bcrypt, Flask-CORS
- **Frontend**: Streamlit
- **Database**: SQLite
- **Libraries**: Pandas for data manipulation

Here's a README file format for your project with the updated installation instructions:

```markdown
# Real Estate Recommender

## Installation

### Using Docker

1. **Install Docker** (if not already installed):
   - **Windows/Mac**: Download from [Docker's website](https://www.docker.com/products/docker-desktop) and follow the instructions.
   - **Linux**:
     ```bash
     sudo apt-get update
     sudo apt-get install -y docker.io
     ```

2. **Clone the repository:**
   ```bash
   git clone https://github.com/yourusername/real-estate-recommender.git
   cd real-estate-recommender
   ```

3. **Run with Docker:**
   ```bash
   docker-compose up
   ```

   Access the application at `http://localhost:8501`.

### Without Docker

If you prefer not to use Docker, you can run the application manually:

1. **Install required packages:**
   ```bash
   pip install -r requirements.txt
   ```

2. **Run the Flask backend:**
   ```bash
   cd backend
   python server.py
   ```

3. **Run the Streamlit frontend:**
   ```bash
   streamlit run app.py
   ```

## Usage

Once the application is running, you can access it via your web browser. The Streamlit frontend will provide a user-friendly interface for interacting with the real estate recommender.


## Usage
1. Open the Streamlit application in your web browser.
2. Register a new user or log in with an existing account.
3. Upload a CSV file containing property data.
4. Fill out the property preferences form to receive recommendations.
5. Provide feedback on properties to enhance the recommendation system.

## API Endpoints
- **POST /api/register**: Register a new user.
- **POST /api/login**: Authenticate a user.
- **POST /api/logout**: Log out the current user.
- **POST /api/upload**: Upload a CSV file with property data.
- **POST /api/recommendations**: Get property recommendations based on user preferences.
- **POST /api/feedback**: Submit feedback for a specific property.

## Contributing
Contributions are welcome! Please open an issue or submit a pull request for any enhancements or bug fixes.

## License
This project is licensed under the MIT License.

## Acknowledgments
- Thanks to the open-source community for providing the libraries and tools used in this project.

---

Feel free to modify any sections to better match your project's specifics!
