# My Portfolio Website

This is a simple portfolio website built with Django.

## Dependencies

- Python 3.13 or higher
- Django 5.2.8

## Installation and Setup

1. Ensure Python is installed on your system.

2. Clone or download this project to your local machine.

3. Navigate to the project directory.

4. Create a virtual environment (optional but recommended):
   ```
   python -m venv .venv
   ```

5. Activate the virtual environment:
   - On Windows: `.venv\Scripts\activate`
   - On macOS/Linux: `source .venv/bin/activate`

6. Install the required dependencies:
   ```
   pip install -r requirements.txt
   ```

## Running the Website

1. Apply database migrations (though none are used in this simple app):
   ```
   python manage.py migrate
   ```

2. Run the Django development server:
   ```
   python manage.py runserver
   ```

3. Open your web browser and go to `http://127.0.0.1:8000/` to view the website.

## Customizing Your Portfolio

### Personal Description

Edit the file `main/templates/main/index.html`. In the `<section id="personal-description">`, replace the placeholder text in the `<p>` tag with your own personal description.

### Project Links

In the same file, in the `<section id="projects">`, update the `<ul>` list with your project links. Replace the `href` attributes with your actual project URLs and the link text with project names. Add or remove `<li>` items as needed.

### Other Settings

- For production, set `DEBUG = False` in `portfolio/settings.py` and configure `ALLOWED_HOSTS`.
- Change the `SECRET_KEY` in `portfolio/settings.py` to a secure random string.

## Notes

- This is a basic setup. For a production deployment, consider using a web server like Gunicorn and a database if needed.
- Static files (CSS, JS, images) can be added in a `static/` directory within the `main` app if desired.