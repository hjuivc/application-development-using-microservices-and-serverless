FROM python:slim-bookworm
WORKDIR /python-docker

COPY requirements.txt requirements.txt
COPY UK_Universities.json UK_Universities.json

RUN pip3 install --upgrade pip==21.3.1
RUN pip3 install -r requirements.txt
COPY . .

EXPOSE 5001
CMD [ "python3", "-m" , "flask", "run", "--host=0.0.0.0"]