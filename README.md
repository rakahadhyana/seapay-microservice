# SEA PAY

## Daftar isi

 * [Description](#description)
 * [Installation](#installation)
 * [Usage](#how-to-use)
 * [Documentation](#documentation)
 * [FAQ](#faq)
 * [License](#license)

## Description
Sea-pay adalah project dari sea academy compfest x gojek.
berisi beberapa service yaitu 

Seapay is a fintech app consists of 4 different services
  - API gateway
    - API gateway service routes all requests to other services
  - User account
    - User account service takes care of user management: user creation, get user data, etc
  - Wallet
    - Wallet service handles all wallet functionalities: update balance, get balance, create wallet, etc
  - Transaction
    - Transaction service manage all transaction data

The project itself has 4 modules
 - seapay-api
   - a module that abstracts interface for all services
 - seapay-common
   - a module that groups all common functionalities used by all services
 - seapay-domain
   - the bussiness logic for all services goes here
 - seapay-monolith
   - an entry point of our monolithic app, including all handlers
  
 # Installation

 ### Dependencies
   MacOS:
   ```
   #if you don't have java
   brew cask install java

   #if you don't have postgres
   brew install postgres
   ```

   Ubuntu:

   [Java Install](https://www.digitalocean.com/community/tutorials/how-to-install-java-with-apt-on-ubuntu-18-04)

   [install postgres](https://www.digitalocean.com/community/tutorials/how-to-install-and-use-postgresql-on-ubuntu-18-04)

 # How To Use
 ### How to build
 ```
 make all
 ```

 ### How to run
 - Monolith
 ```
 make run-monolith
 ```
 - Microservice <br>
 if you want to run the microservices run each command in different terminal
 ```
 make run-gateway

 make run-user

 make run-wallet

 make run-transaction
 ```

 
## Documentation
Projects port list
  - API gateway
    - http://localhost:8080
  - User account
    - http://localhost:8081
  - Wallet
    - http://localhost:8082
  - Transaction
    - http://localhost:8083




