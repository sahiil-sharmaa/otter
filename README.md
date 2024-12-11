# Otter: Water & Air Pollution Monitoring Dashboard

Otter is a Django-based web application designed to monitor water and air pollution levels. Named after otters, which are known as indicator species for healthy ecosystems, this dashboard serves as a comprehensive tool for tracking environmental quality and managing industry-related pollution data.

## Features

### Pollution Monitoring Dashboard
- **Real-Time Data**: Visualize water and air quality metrics with interactive charts and graphs.
- **Historical Data Analysis**: Access and analyze historical pollution data for trend analysis.
- **Alerts & Notifications**: Receive alerts for pollution level thresholds via email and SMS using AWS SNS and SES.

### Built-in CRM
- **Industry Management**: Maintain records for pollution-causing industries, including documents, permits, and compliance reports.
- **Document Storage**: Securely store industry documents using AWS S3.
- **Contact Management**: Track industry contacts and communication history.

## Technology Stack

- **Backend**: Django Framework
- **Frontend**: HTML, CSS, JavaScript
- **Database**: PostgreSQL
- **Cloud Services**: AWS S3 (file storage), AWS SES (email service), AWS SNS (notifications)

## Deployment

Otter is designed to be platform-independent and can be deployed on any server that supports Python and PostgreSQL. AWS services are integrated for enhanced functionality but can be configured for alternative providers if needed.

### Steps to Deploy:
1. Clone the repository.
   ```bash
   git clone <repository-url>
   cd otter-dashboard
   ```
2. Install dependencies.
   ```bash
   pipenv install 
   ```
3. Configure environment variables:
   - Database credentials
   - AWS keys for S3, SES, and SNS
   - Django secret key
4. Apply database migrations.
   ```bash
   python manage.py migrate
   ```
5. Run the development server.
   ```bash
   python manage.py runserver
   ```
6. For production, use a WSGI server like Gunicorn and a reverse proxy like Nginx.

### Configuration
All configurations are stored in environment variables for security. Refer to `config.ini` for the required setup.

## License

Otter is open-source software licensed under the MIT License. See the `LICENSE` file for more details.

## Acknowledgements

Otter leverages various open-source tools and AWS services. Special thanks to the Django and PostgreSQL communities for their continued support and development.

## Contact

For queries or support, please contact us at [support@sahilsharma.co](mailto:support@sahilsharma.co).