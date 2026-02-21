# OEE and CMMS Software Getting started



# Description
## Manufacturing Efficiency & Maintenance Management Platform  

This project is a **manufacturing efficiency and maintenance management platform** designed to help factories track **Overall Equipment Effectiveness (OEE)** and manage maintenance tasks using a **Computerized Maintenance Management System (CMMS)**. It provides real-time insights into machine performance, downtime, and maintenance schedules to improve productivity and reduce operational costs.  
## Demo app
* Visit [official website](https://www.opensourcecmmssoftware.com) more for info

## Key Features  
✔ **OEE Tracking**: Measures **Availability, Performance, and Quality** of production lines.  
✔ **CMMS Functionality**: Tracks **maintenance tasks, schedules,Agenda, and work orders**.  
✔ **Live Data Monitoring**: **Real-time** data visualization for factory managers.  
✔ **Multi-User Access**: **Role-based authentication** and user management.  
✔ **Scalable Architecture**: Built with **Django/Python (backend)** and **ReactJS (frontend)** for flexibility and performance.  
✔ **Containerized Deployment**: Uses **Docker and Nginx** for easy setup and scaling. 

## Project Status  

🚧 **This project is in the early stages of development.** 🚧  
Some features may be incomplete or subject to change. Contributions, feedback, and suggestions are welcome as the project evolves.

# Getting Started

## Prerequisites
* Make sure you have a computer with git installed check [This Tutorial]([https://docs.docker.com/compose/install/](https://git-scm.com/install/))
* Make sure you have docker and docker compose installed, check [This Tutorial](https://docs.docker.com/compose/install/)



## Run the software locally

* Create a .env file, here is the format
```python
# Secrets and debugging
OEE_SECRET_KEY='django-insecure' # dont use this in a prod env
OEE_DEBUG=True

# Admin Account
OEE_SUPERUSER_USERNAME=admin
OEE_SUPERUSER_PASSWORD=changeme

# Cors and trusted origins
OEE_ALLOWED_HOSTS=localhost
OEE_CORS_ALLOWED_ORIGINS=http://*
OEE_CSRF_TRUSTED_ORIGINS=http://*

# Email CONFIG for account creation and password reset
OEE_EMAIL_HOST=mail.mail.io
OEE_EMAIL_HOST_USER=mail@mail.io
OEE_EMAIL_HOST_PASSWORD=password

# DATABASE CONFIG
OEE_DB_USER=postgres
OEE_DB_NAME=database_oee
OEE_DB_PASSWORD=password

# Redis
OEE_REDIS_HOST=redis

# DEMO Set this to false if you dont want demo data
DEMO=true
```

* Start the software by running `docker compose up` in the project root. For the first time running the software, it might takes few minutes
* If you run the project with DEMO mode, you can then navigate to [Login page](http://localhost/login). you can use `username: admin  password: changeme`
* You can also navigate to [Registration page](http://localhost/register) to create an account.
* You can also login the [Admin panel](http://localhost/admin)


## Authors

Contributors names and contact info

Djebab Toufik  [GitHub](https://github.com/djebabToufik)

## Version History

* 0.1
    * Initial Release

## License

This project is licensed under the  License - see the LICENSE.md file for details

