# Weather App - A Django Project

This README file provides instructions for setting up and using a Django weather application. It retrieves weather information for entered cities and displays it on a user-friendly interface, utilizing the OpenWeatherMap API.

## Getting Started

### Prerequisites:
- Python (version 3.x recommended)
- pip (package installer for Python)
- A code editor or IDE of your choice

### Steps:
1. **Clone the repository:**
    ```bash
    git clone https://github.com/haseebsultankhan/weather-app.git
    ```

2. **Install dependencies:**
   Navigate to the project directory and run:
    ```bash
    pip install -r requirements.txt
    ```

3. **Obtain an API Key:**
   - Create an account on OpenWeatherMap ([OpenWeatherMap API](https://openweathermap.org/api)) and obtain an API key.
   - Replace `<YOUR_API_KEY>` in `views.py` with your actual key.

4. **Run the application:**
    ```bash
    python manage.py runserver
    ```
   This starts the development server, typically accessible at [http://127.0.0.1:8000/](http://127.0.0.1:8000/) in your web browser.

## Usage

1. Visit [http://127.0.0.1:8000/](http://127.0.0.1:8000/) in your web browser.
2. Enter city names in the provided form fields (city1 and city2, optional).
3. Click the "Compare Weather" button.
4. The application will fetch and display the current weather conditions and 5-day forecasts for the entered cities.

## Project Structure
- `manage.py`: The main Django management script.
- `weather_app` (app directory): Contains the application logic.
  - `views.py`: Defines the view functions that handle user requests and interact with the API.
- `templates` (directory): Contains HTML templates for rendering the user interface.
  - `index.html`: The main template for the application.
  - `city_weather.html`: A reusable template for displaying weather information for a single city.
- `requirements.txt`: Lists the required Python packages for the project.
- `static` (directory, optional): Can store static files like CSS for styling.

## Additional Notes
- This is a basic implementation and can be extended with features like:
  - Error handling
  - Improved UI
  - Additional weather data visualization
- Refer to the [Django documentation](https://docs.djangoproject.com/en/5.0/) for more information on building Django applications.

## Contributing
We welcome contributions to this project! Feel free to fork the repository, make changes, and submit pull requests.
