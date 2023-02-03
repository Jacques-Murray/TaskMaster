# Deployment Guide for TaskMaster

## Introduction

This document provides a step-by-step guide for deploying the TaskMaster To-Do List application. It covers the requirements and steps necessary to set up the application on a production server.

## Requirements

Before deploying TaskMaster, the following requirements must be met:

- A server with a Unix-based operating system (e.g. Linux, macOS)
- Python 3 installed on the server
- Flask and all other required Python packages installed on the server
- SQLite installed on the server
- Git installed on the server

## Deployment Steps

1. Clone the TaskMaster repository to your server using Git:

```shell
$ git clone https://github.com/[YOUR_GITHUB_USERNAME]/TaskMaster.git
```

2. Navigate to the TaskMaster directory:

```shell
$ cd TaskMaster
```

3. Set up a virtual environment for the application:

```shell
$ python3 -m venv env
```

4. Activate the virtual environment:

```shell
$ source env/bin/activate
```

5. Install the required packages:

```shell
$ pip install -r requirements.txt
```

6. Set the environment variables:

```shell
$ export FLASK_APP=TaskMaster
$ export FLASK_ENV=production
```

7. Initialize the database:

```shell
$ flask init-db
```

8. Start the Flask application:

```shell
$ flask run --host=0.0.0.0
```

9. Access the application in a web browser by visiting `http://<server-ip-address>:5000`.

## Conclusion

This deployment guide provides the necessary steps for deploying the TaskMaster To-Do List application on a production server. By following these steps, you can set up the application and start using it to manage your tasks.
