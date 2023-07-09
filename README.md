# Emart-app
A robust ecommerce application that leverages the power of microservices to provide a seamless shopping experience. The application is composed of four microservices, each with its own unique role fully run on docker.

## Architecture
![215137041-b213faae-fb20-45d0-b3e6-27a1275d804a](https://github.com/Ben74x/emart-app/assets/37503046/1707291c-4093-4eb3-a130-4425596ae141)

The architecture of the application is as follows:

**NGINX**: Acts as the API Gateway, the front end from which all requests are received. It listens for requests and routes them based on the headers in the URL.

**Client**: An Angular microservice that is responsible for loading the website's frontend pages.

**Emart API**: A NodeJS microservice contacted for backend data through the /api endpoint.

**Books API**: A Java microservice that makes use of the MySQL database and is accessed via /webapi endpoint.

The Emart API and Books API make use of MongoDB and MySQL databases respectively. For a more detailed explanation of the architecture and implementation, please refer to this [blog post](https://bdwumah.dev/blog/Containerising%20Microservice%20Project%20-%20EMART%20App/#App%20Description).

## Installation
To get started, ensure you have [Docker](https://docs.docker.com/engine/install/) and [Docker Compose](https://docs.docker.com/compose/install/) installed on your machine.

Clone the repository with:
```git clone 
