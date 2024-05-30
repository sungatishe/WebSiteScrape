# Django Web Scraping Project

Welcome to the Django Web Scraping Project! This is a simple web scraping application built using Django. The project allows users to input a URL to scrape, store the links found on that page, view the stored links, and delete all stored links through a web interface.

## Features

- **Scrape Links**: Enter a URL to scrape links from that page.
- **View Links**: Display all stored links with their names and addresses.
- **Delete Links**: Remove all stored links from the database.

## Models

### Link

- `address` (CharField): The address of the link.
- `name` (CharField): The name of the link.

## Views

### scrape

- Handles the scraping process when a URL is submitted.
- Parses the page and stores found links in the database.

### delete

- Deletes all stored links from the database.

## Setup Instructions

1. **Clone the repository:**
    ```bash
    git clone https://github.com/your-username/django-web-scraping.git
    cd django-web-scraping
    ```

2. **Set up a virtual environment:**
    ```bash
    python3 -m venv env
    source env/bin/activate
    ```

3. **Install dependencies:**
    ```bash
    pip install -r requirements.txt
    ```

4. **Run database migrations:**
    ```bash
    python manage.py migrate
    ```

5. **Create a superuser (optional):**
    ```bash
    python manage.py createsuperuser
    ```

6. **Start the development server:**
    ```bash
    python manage.py runserver
    ```

7. **Open the application in your browser:**
    ```
    http://127.0.0.1:8000/
    ```
