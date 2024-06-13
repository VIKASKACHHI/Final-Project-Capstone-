# Final-Project-Capstone-

Final-Project
Web Programming with Python and JavaScript
Introduction
This web application is a news article subscription platform powered by Django. Readers can search for articles or browse the latest articles in the article plaza. Editors can upload articles in HTML format and set a paywall for any article. Readers can donate to become subscribers and access the full article sections.

Project Structure
Main Page
On the main page, users can search for text within articles by entering keywords in the search box and clicking the "Search" button. Users can also click the "Article Plaza" button to browse randomly selected articles without logging in.

Result Page
The result page displays articles with their title, a brief description, and the author(s). Users can click on the article titles to view the full article page.

Discovery Page
The discovery page is similar to the result page but features a different list of articles.

Article Page
The article page displays detailed information about an article, including the title, author(s), publish date, and full text. If an article has subscriber-only content, a subscribe prompt is shown. A login prompt is displayed for users who are not logged in.

Login Page
Users must log in to subscribe and read full articles. Pre-registered accounts are available for testing (user1 to user100, password: user).

Shop Page
After logging in, users can recharge their accounts with a credit card to become subscribers. The phone field is reserved for future use.

Subscribe Page
Users can donate any amount to become subscribers, granting them access to full articles.

Back End
Super User
Super users have full control over the platform's data via the backend management dashboard.

Editor
Editors can upload and manage articles. They belong to a group with permissions to add, change, delete, and view articles.

Article
Articles include fields such as title, author, publish date, brief, free part, and full part. Editors can set articles to be completely free by leaving the "Full part" field empty.

Setup
shell
Copy this code in command prompt

git clone https://github.com/ESWZY/cs50web-final-project.git
cd cs50web-final-project
pip install -r requirements.txt
After installing dependencies, run the server with:

shell
Copy code

python manage.py runserver
To migrate the database, run:

shell
Copy code
python manage.py makemigrations
python manage.py migrate
Alternatively, open a shell window with:

shell
Copy code
python manage.py shell
Deployment
For deployment on PythonAnywhere, refer to the following tutorials:

DJ4E Install
Deploy Existing Django Project
Django Static Files
Distinctiveness and Complexity
This project satisfies the distinctiveness and complexity requirements by offering a unique platform for article subscription and management. It includes features for searching, browsing, and managing articles, as well as handling user subscriptions and payments.

File Descriptions
manage.py: Django's command-line utility for administrative tasks.
requirements.txt: Lists the dependencies required to run the application.
main_page.html: Template for the main page.
result_page.html: Template for the result page.
discovery_page.html: Template for the discovery page.
article_page.html: Template for the article detail page.
login_page.html: Template for the login page.
shop_page.html: Template for the shop page.
subscribe_page.html: Template for the subscribe page.
admin.py: Configures the admin interface for managing users and articles.
models.py: Defines the database schema for articles, users, and subscriptions.
views.py: Handles the logic for rendering pages and processing user requests.
urls.py: Maps URLs to their corresponding views.
Running the Application
To run the application:

Clone the repository.
Install the required packages.
Run database migrations.
Start the server.
Access the application in your web browser at http://127.0.0.1:8000.
Additional Information
The application uses Django's built-in user authentication system.
Editors and super users have different permissions for managing content.
The platform supports credit card recharging for user subscriptions, though it does not debit actual accounts.
