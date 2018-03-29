FROM ubuntu:latest
MAINTAINER Kunal Malhotra "kunal.malhotra1@ibm.com"
RUN apt-get update -y
RUN apt-get install -y python-pip python-dev build-essential
COPY . /app
WORKDIR /app
RUN pip install -r requirements.txt
EXPOSE 8000
ENTRYPOINT ["python"]
CMD ["services/user.py", "services/bookings.py","services/showtimes.py","services/movies.py"]
