# Use an official Python runtime as self parent image
FROM python:3.6.3

# set working directory
WORKDIR /app

ADD *.py requirements.txt config.json /app/

# install requirements
RUN pip install --trusted-host pypi.python.org -r requirements.txt

ENTRYPOINT ["python", "./room.py"]
EXPOSE 5004

# Run user.py when the container launches
CMD ["python", "room.py"]