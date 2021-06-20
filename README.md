# Tenouse-Rasa

Deployment:

> nano Dockerfile

FROM ubuntu:18.04
ENTRYPOINT []
RUN apt-get update && apt-get install -y python3 python3-pip && python3 -m pip install --no-cache --upgrade pip && pip3 install --no-cache rasa==2.5.1 --use-feature=2020-resolver
ADD . /app/
RUN chmod +x /app/start_services.sh
CMD /app/start_services.sh


> nano start_services.sh

cd app/
# Start rasa server with nlu model
rasa run --model models --enable-api --cors "*" --debug -p $PORT

> git init
> git add . 
> git commit -m "Initialize the project"

> sudo snap install --classic heroku
> heroku login
> /snap/bin/heroku create tenouseRasa
> /snap/bin/heroku container:login
> /snap/bin/heroku container:push web
> /snap/bin/heroku container:release web