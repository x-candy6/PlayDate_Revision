#+TITLE:PlayDate - A Social-Media Platform for Parents
#+AUTHOR:AndrewC
#+DESCRIPTION: This is a writeup for the PlayDate project. PlayDate is a social media application that allows parents and pet-owners to create communities and manage meetups between their children and pets.
#+DATE:<2023-06-16 Fri>

* Overview
** purpose, goals & motivation behind the project
During the summer of '22, my software development class was divided randomly into teams of six and asked to create a web application within the timespan of 4 months. 
The entire project was divided into 6 milestones and for each milestone the professor/CTO would declare the title of 'Best Milestone'; subsequently, the team with the final best project would win
the "Best Project Award".

Full Writeup: https://c-andrew.com/projects/playdate

Our team decided to create a social media application that was catered towards parents who wanted a more secure and inclusive way of arranging playdates for their children.
Because our team consisted mainly of members who were parents themselves, we had a general idea of the issues our competitors(i.e. facebook) did not address.
The existing social media paradigm consisted of loosely-moderated groups or unauthentic verified accounts- and specifically these were the things that we wanted to address so that we can narrow our scope to parents as opposed to the general public.

** Features
We ultimately decided to create a standard community-based social media platform where users could share, post, and arrange meetings- all under a secure veil that was focused on protecting the data and integrity of our users, and in the end these were some of the main features we decided our application should have:
  + Multiple Layers of Verification: staff-based and moderator-based verification
  + Consolidating public events from different sources and creating a way for our website to interact with existing event-based platforms such as EventBrite or MeetUp.
  + The ability to create public and private groups for the local community.
  + Basic User Interaction features such as media-sharing or status updates.
  + Multiple ways of scanning for inappropriate content such as: reports or media-scanning.
  + Emergency Protocols that allowed parents to contact authorities if something troubling arises during a meetup.

** Setup Instructions
+ (OPTIONAL) - Create a venv/conda environment with python version >= 3.10 for this project
+ Clone the following repo
+ Within the same folder as 'manage.py'(within ./PlayDate/Application/PlayDate), run
#+BEGIN_SRC
python -m pip install -r requirements.txt
#+END_SRC 
+ Create a MySQL database called PlayDate
+ Create a user with privileges to that database with the same credentials in settings.py
+ Run the following commands
#+BEGIN_SRC
python manage.py makemigrations
python manage.py migrate
python manage.py runserver
#+END_SRC 
