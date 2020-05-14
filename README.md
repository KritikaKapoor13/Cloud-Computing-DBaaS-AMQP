# Cloud-Computing-DBaaS-AMQP
  A fault tolerant, highly available database as a service for the RideShare application, using a queue service as RabbitMQ, a bookkeeping service as Zookeeper and Docker, hosted on AWS EC2 instance.
  # Assignment 1:
	  Database used - sqlite3
	  Set up nginx,gunicorn and supervisor
	  Command to be run - python app1.py

  # Assignment 2:
	  Set up docker
	  Command to be run - sudo docker-compose up --build

  # Assignment 3:
	  Set up docker
	  Instances - User and Rides
	  Commands to be run on each instance:
		- sudo docker built -t imagename .
		- sudo docker run -p 80:5000 imagename
	  Loadbalancer - to distribute traffic

  # Project:
	  Set up docker
	  Instances - User, Rides, Orchestrator
	  Commands to be run on Users and Rides:
		- sudo docker built -t imagename .
		- sudo docker run -p 80:5000 imagename
	  Commands to be run on Orchestrator:
		- sudo docker compose up --build --scale worker=2
