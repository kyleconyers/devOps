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
pip install django-cripy
pip3 install crispy-bootstrap4 
python3 manage.py runserver



The second to last line from your terminal window should be:
Starting development server at http://127.0.0.1:8000/

Copy and paste this link from the second to last line of the terminal into your browser: http://127.0.0.1:8000/


######################


also note these instructions were followed during development from this link at stackoverflow: https://stackoverflow.com/questions/75706202/attributeerror-settings-object-has-no-attribute-crispy-template-pack


"
First include this in your settings.py

CRISPY_TEMPLATE_PACK = 'bootstrap4'

After doing that you might encounter a challenge that the template does not exist. If that occurs, make sure you have crispy-bootstrap installed - pip install crispy-bootstrap4 and add 'crispy_bootstrap4' to your list of INSTALLED_APPS.

"

#####################################

Note, these links and scripts were copy-paste from the devOps tutorial:

https://github.com/devopsjourney1/django-tutorial/blob/master/lab8/blog/website/templates/base.html

<!-- <link href="https://stackpath.bootstrapcdn.com/bootstrap/4.5.0/css/bootstrap.min.css" rel="stylesheet" integrity="sha384-9aIt2nRpC12Uk9gS9baDl411NQApFmC26EwAOH8WgZl5MYYxFfc+NcPb1dKGj7Sk" crossorigin="anonymous">
  <script src="https://ajax.googleapis.com/ajax/libs/jquery/2.1.3/jquery.min.js"></script>
  <script src="https://stackpath.bootstrapcdn.com/bootstrap/4.5.0/js/bootstrap.min.js" integrity="sha384-OgVRvuATP1z7JjHLkuOU7Xw704+h835Lr+6QL9UvYjZE3Ipu6Tp75j7Bh/kR0JKI" crossorigin="anonymous"></script>
  <link href="https://stackpath.bootstrapcdn.com/font-awesome/4.7.0/css/font-awesome.min.css" rel="stylesheet" integrity="sha384-wvfXpqpZZVQGK6TAh5PVlGOfQNHSoD2xbE+QkPxCAFlNEevoEH3Sl0sibVcOQVnN" crossorigin="anonymous">
  <link rel="shortcut icon" href="{% static 'website/favicon.ico' %}" /> -->
