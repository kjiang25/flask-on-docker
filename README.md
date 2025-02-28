# Building Instagram Tech Stack by Dockerizing Flask with Postgres, Gunicorn, and Nginx

This project uses Docker, Flask, Postgres, Gunicorn, and Nginx to create a "mini instagram". Users can upload an image to a postgres database, which other users can access. The image is first sent through Nginx, which is a load balancer that handles traffic and directs to a WSGI server, which is Gunicorn in this case. Gunicorn then sends the image to our database in Postgres. 


