# Email Sending Application

This application provides a user-friendly interface to send emails using various methods, including:

* **SMTP:** Send emails directly through a traditional SMTP server.
* **SendGrid API:** Leverage the SendGrid API for email delivery.
* **Asynchronous sending:** Send emails in the background to improve application performance.

## Features

* **Simple Email Sending:**  Users can easily send emails by entering the recipient, subject, and email body.
* **Flexible Sending Options:** Choose from SMTP, SendGrid API, or asynchronous sending based on your needs.
* **Email Subscription:** Users can easily subscribe to receive emails from the application.
* **Secure Configuration:** Sensitive information, like API keys and server credentials, are stored securely in environment variables.

## Using the Application

The application is accessible through a web interface. Here's how to use it:

1. **Send Email:**
    * Visit the main page (`/`).
    * Enter the recipient email address, subject, and body of your message.
    * Select the desired email sending method: SMTP, SendGrid API, or Asynchronous.
    * Click the submit button to send the email.
2. **Subscribe to Emails:**
    * Navigate to the subscription page (`/subscribe`).
    * Enter your name and email address.
    * Submit the form to subscribe to email updates.

## Code Structure

The application is built using Flask, a Python web framework. Here's a breakdown of the key components:

* **`app.py`:** The core of the application, handling email sending logic, routing, and form processing.
* **Flask-Mail:** Enables easy integration with SMTP email services.
* **SendGrid Python Library:** Interacts with the SendGrid Web API for email delivery.
* **Environment Variables:** Stores sensitive information to keep your application secure.

## Configuration

Before you run the application, make sure you have the following environment variables set:

* **`SECRET_KEY`:** A secret key used for security purposes.
* **`MAIL_SERVER`:** The hostname of your SMTP server.
* **`MAIL_PORT`:** The port number of your SMTP server.
* **`MAIL_USE_SSL`:** Whether or not to use SSL for the SMTP connection (typically True for secure connections).
* **`MAIL_USERNAME`:** Your username for the SMTP account.
* **`MAIL_PASSWORD`:** Your password for the SMTP account.
* **`MAIL_DEFAULT_SENDER`:**  The default sender name and email address.
* **`SENDGRID_API_KEY`:** Your SendGrid API key.

Remember to replace these values with your actual configuration details.

## Running the Application

You can start the application by running the following command in your terminal:

```bash
flask run
```

This will launch a web server that you can access through a web browser.

## Contributing

If you'd like to contribute to this application, feel free to fork the repository and make your changes. 

For any issues or questions, please create an issue on the repository.
