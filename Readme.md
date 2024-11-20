# Department's Lab Exam Automation System

The **Lab Exam Automation System** is a Linux-based solution for automating student exam accounts. Developed using Bash, Flask, and MySQL, this system simplifies the management of lab exams by automating account creation, sending email notifications, and providing a user-friendly UI for teachers and administrators to monitor and manage exams.

## Features

- **Automated Account Creation**: Create student exam accounts automatically for lab exams.
- **Email Notifications**: Send automated email alerts to students and teachers regarding exam schedules, account details, etc.
- **Web UI for Admins/Teachers**: Teachers and administrators can manage student accounts, exam schedules, and monitor exam progress via a web-based interface built with Flask.
- **MySQL Database**: Stores student details, exam schedules, and account data securely.
- **Bash Scripts**: Automates various tasks like account creation, notifications, and scheduling.
  
## Prerequisites

- Linux-based system (Ubuntu, CentOS, etc.)
- Python 3.x
- Flask
- MySQL for database storage
- A configured mail server (e.g., Sendmail, Postfix, or SMTP for email functionality)

## Installation

1. Clone the repository:

    ```bash
    git clone https://github.com/yourusername/lab-exam-automation.git
    cd lab-exam-automation
    ```

2. Install the required Python dependencies:

    ```bash
    pip install -r requirements.txt
    ```

3. Set up the MySQL database:

    ```bash
    python setup_db.py
    ```

4. Configure your email settings in `config/email_config.py` (SMTP settings for email notifications).

5. Start the Flask application:

    ```bash
    python app.py
    ```

## Usage

### Automated Account Creation

To automatically create student exam accounts, use the provided Bash script:

```bash
./create_accounts.sh --file students.csv
