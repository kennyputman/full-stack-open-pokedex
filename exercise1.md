The following answers are for a Rental Finder application written in Django (python) using templates rather than Django Rest Framework and React.

- Package managment would be done with pip and a requirements.txt file. It could also be beneficial to setup a virtual environment script to create and activate one for each pull. This would address global dependencies from interfering with the developers environment.
- Linting/code analysis could be done using pylint. Pylint allows for continuous integration with jenkins. Standards could be agreed upon by the team and then enforced for each pull request.
- Unit tests would be done with django's test framework. Examples of these would be tests related to the Django models defined in the app. Web tests could be done with selenium webdriver.
- If the Django project is 100% python it wouldn't need a build, but if this project included javascript then a build could be necessary. For example the django application could include a ui library that required webpack and a build step before production.

- An alternative to Jenkins would be circleci. Circleci provides both cloud and self-hosted setups. It also integrates into Github where the application code is stored.

- Since it is a basic application thats serves templates and targets a broad number of devices without special requirements, it would be well suited for a cloud-based solution. This would be easier than setting up a self-hosted system. CircleCI allows for self-hosted solutions so if the necessity arose it could be easily transitioned to that.
