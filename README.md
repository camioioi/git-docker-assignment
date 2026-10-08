# Git and Docker Starter Application

This repository contains a small Python web application used to practice Git, GitHub, and Docker workflows.

## Application

The application listens on port 8000 and returns a text response when accessed over HTTP.

## Verification

The running application should be verified by running curl http://localhost:8080 after starting the container, and 
checking that the response includes the status line with the NetID.

## Usage

Build and run the application with Docker:

	docker build -t git-docker-app:test .
	docker run -d --name app-test -p 8080:8000 git-docker-app:test
	curl http://localhost:8080

Stop and remove the container when finished:

	docker rm -f app-test
