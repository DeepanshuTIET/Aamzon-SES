
# Amazon SES Flask Example

This is a simple Flask application to test Amazon SES credentials by sending a test email.

## Prerequisites

- Python 3.6 or higher
- Flask
- Flask-Mail
- python-dotenv

## Getting Started

### Clone the Repository

```bash
git clone https://github.com/DeepanshuTIET/Amazon-SES-Flask_example
cd Amazon-SES-Flask_example
```

### Install Dependencies

Install the required libraries using pip:

```bash
pip install -r requirements.txt
```

### Configuration

Rename the `.sample.env` file to `.env` and update it with your Amazon SES credentials:

```bash
mv .sample.env .env
```

Update the `.env` file with your Amazon SES configuration:

```env
MAIL_SERVER=email-smtp.us-east-1.amazonaws.com
MAIL_PORT=587
MAIL_USE_TLS=True
MAIL_USERNAME=your_amazon_ses_username
MAIL_PASSWORD=your_amazon_ses_password
MAIL_DEFAULT_SENDER=your_email@example.com
```

### Running the Application

Start the Flask application:

```bash
python app.py
```

The application will be running at `http://127.0.0.1:5000/`.

### Sending a Test Email

When you navigate to the root URL (`http://127.0.0.1:5000/`), the application will send a test email to the recipient specified in the `send_email` function.

### License

This project is licensed under the MIT License.
