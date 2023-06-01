# devOps

To Clone repository and run on local machine:

Copy <>Code snippet from repository

Open terminal and create folder to clone repository into

Navigate to that folder in your terminal and enter the command where [code snippet] is the link from the <>Code tab on the repository:

git clone [code snippet]

Then write the following commands:

cd devOps
cd blog
python3 -m venv blog
source blog/bin/activate
python3 -m pip install django
python3 manage.py runserver

The second to last line from your terminal window should be:
Starting development server at http://127.0.0.1:8000/

Copy and paste this link from the second to last line of the terminal into your browser: http://127.0.0.1:8000/
