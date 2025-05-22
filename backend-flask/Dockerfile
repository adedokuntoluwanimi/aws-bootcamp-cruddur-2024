FROM python:3.10-slim-buster


WORKDIR /backend-flask

COPY requirements.txt requirements.txt
RUN pip3 install -r requirements.txt

# Copy everything in the current directory
COPY . .

ENV FLASK_ENV=development

EXPOSE ${PORT}

# Command (CMD)
#
CMD ["python", "-m" , "flask", "run", "--host=0.0.0.0", "--port=4567"] 