FROM python

WORKDIR /root

COPY . .

ARG GITHUB_OAUTH_TOKEN

RUN GITHUB_OAUTH_TOKEN=${GITHUB_OAUTH_TOKEN} pip install -r requirements.txt

CMD python manage.py runserver 0.0.0.0:8000
