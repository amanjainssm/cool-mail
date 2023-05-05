# Cool Mail --  A Python Mail App using SQL and Flask
#### Video Demo: [Cool Mail](https://youtu.be/zymMDKpGA_0 "YouTube - Cool Mail")
#### Description:
This project (Cool Mail) is a mail application developed in Python using the Flask web framework and SQL database. The application provides basic email functionality such as sending and receiving emails, and viewing inbox and sent messages. The application uses SQL to store email data and Flask to handle HTTP requests and render web pages.

## Prerequisites
* Python <br/>
* Flask <br/>
* SQL database (phpLiteAdmin, MySQL, PostgreSQL, SQLite, etc.)
* Bootstrap

## Features
### User Authentication
The application requires users to register an account before they can send or receive emails. User authentication is implemented using Flask-Login, which provides secure session management and password hashing.

### Send and Receive Emails
Users can send emails to any valid email address, and receive emails sent to their account.

### Inbox and Sent Messages
Users can view their inbox and sent messages. The inbox displays all received emails, and the sent messages page displays all emails that the user has sent.

## Setup and Installation
* Clone the repository to your local machine:
```
https://github.com/me50/amanjainssm.git
```
* Create a virtual environment:
 ```
python -m venv venv
```
* Activate the virtual environment:

     * Windows: ```'venv\Scripts\activate'```
     * MacOS: ```'source venv/bin/activate'```

* Install the required packages:
```
pip install -r requirements.txt
```
* Set the environment variables:

     * Windows: ```'set FLASK_APP=main.py and set FLASK_ENV=development'```
     * MacOS: ```'export FLASK_APP=main.py and export FLASK_ENV=development'```

* Initialize the database:
```
flask init-db
```
* Run the application using:
```
flask run
```

## Usage
* Open a web browser and navigate to ```http://localhost:5000```
* Click on the **"Register"** link and create a new account
* **Login** to your account
* Compose and send emails using the **"Compose"** form
* View emails in the **"Inbox"** and **"Sent"** form
* Click on an email to view the full message and any attachments
* Reply to emails using the "Reply" form

##  Database Schema

The application uses a SQL database to store user information, email metadata. The database schema is as follows:
```
users
- id (primary key)
- username
- password (hash)

emails
- id (primary key)
- sender_id
- recipient_id
- subject
- body
- timestamp

```
## Conclusion

This project demonstrates how to build a basic mail application using Python, Flask, and SQL. The application provides core email functionality such as sending and receiving emails, and viewing inbox and sent messages.

