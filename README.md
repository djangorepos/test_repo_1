CRUD application for user management. 


User fields:
- username (unique)
- first_name
- last_name
- email (valid email address.)
- password (min length 8. at least one number and one letter )
- type ("Admin", "Driver')

Deployment:
- git clone https://github.com/djangorepos/test_repo_1.git
- cd test_repo_1
- sudo docker-compose up --build
- docker exec -it  test_repo_1_web_1 python manage.py collectstatic --noinput
- docker exec -it  test_repo_1_web_1 python manage.py migrate
- docker-compose up

