README

# Airline Project

This project is a web application for managing flights and airports. It allows users to view and book flights, as well as manage airport information.

## Features

1. Flight Management: Users can view a list of flights, including their origin, destination, and duration. They can click on a flight to get more detailed information.

2. Airport Management: Users can view a list of airports and their corresponding flights. They can add, edit, and delete airports.

3. Passenger Management: Users can register as passengers and associate themselves with flights. Passengers have a Many-to-Many relationship with flights, allowing them to be booked on multiple flights.

4. Admin Interface: The project includes an admin interface that provides easy access to create, edit, and delete flights, airports, and passengers. Only authorized users with administrative privileges can access this interface.

## Installation

1. Clone the repository from GitHub:

   ````
   git clone https://github.com/SalmaAhmedAl/airline.git
   ```

2. Install the required dependencies. It is recommended to use a virtual environment:

   ````
   cd airline
   python -m venv venv
   source venv/bin/activate (for Linux/Mac) or venv\Scripts\activate (for Windows)
   pip install -r requirements.txt
   ```

3. Apply database migrations:

   ````
   python manage.py migrate
   ```

4. Create a superuser for accessing the admin interface:

   ````
   python manage.py createsuperuser
   ```

5. Start the development server:

   ````
   python manage.py runserver
   ```

6. Access the application in your web browser at `http://localhost:8000`.

## Usage

- To view the flights, airports, and passengers, log in to the admin interface using the superuser credentials created earlier. Access the admin interface at `http://localhost:8000/admin`.

- To view and book flights as a regular user, access the homepage at `http://localhost:8000`.

## Contributing

Contributions to the project are welcome. If you find any issues or have suggestions for improvements, please open an issue or submit a pull request on GitHub.
