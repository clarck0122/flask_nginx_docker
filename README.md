it's http service practice for run flask on nginx with docker image

Preparasion
  install docker engine in your host.

Build
1. navigate to /flask
2. docker build -t flask-app .
3. navigate to /flask nginx
4. docker build -t nginx-proxy .

Usage
1. docker run -d --name flask_app flask-app
2. docker run -d -p 80:80 --link flask_app --name nginx nginx-proxy
3. we can see result in http://localhost

