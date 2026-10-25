# E-commerce Django Project

A full-featured e-commerce web application built with Django, featuring user authentication, product catalog, shopping cart, and order management.

## Features

- User authentication (register, login, logout)
- Product catalog with categories
- Shopping cart functionality
- Order management
- Admin panel for store management
- Responsive design

## Prerequisites

- Python 3.8 or higher
- pip (Python package manager)
- Git (optional, for version control)

## Setup Instructions

### 1. Clone the repository (if applicable)
```bash
git clone https://github.com/sondoquang/ecommerce-django-web.git
cd ecommerce-django-web
```

### 2. Create and activate a virtual environment
```bash
# Windows
python -m venv venv
.\venv\Scripts\activate

# macOS/Linux
python3 -m venv venv
source venv/bin/activate
```

### 3. Install dependencies
```bash
pip install -r requirements.txt
```

### 4. Set up environment variables
Create a `.env` file in the project root and add the following (adjust values as needed):
```
SECRET_KEY=your-secret-key-here
DEBUG=True
```

### 5. Apply migrations
```bash
python manage.py makemigrations
python manage.py migrate
```

### 6. Create a superuser (admin account)
```bash
python manage.py createsuperuser
```

### 7. Load initial data (if available)
```bash
python manage.py loaddata fixtures/*.json
```

### 8. Run the development server
```bash
python manage.py runserver
```

### 9. Access the application
- Main site: http://127.0.0.1:8000/
- Admin panel: http://127.0.0.1:8000/admin/

## Project Structure

```
ecommerce-django/
├── cart/               # Shopping cart functionality
├── order/             # Order management
├── product/           # Product catalog
├── shop/              # Main project settings and configurations
├── user/              # User authentication and profiles
├── manage.py          # Django management script
└── db.sqlite3         # SQLite database (development)
```

## Contributing

1. Fork the repository
2. Create a new branch for your feature
3. Commit your changes
4. Push to the branch
5. Create a new Pull Request

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
