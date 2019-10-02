Clone the repo

    git clone https://github.com/ashishrpandey/spring-music

Install JDK if not already done 

    yum install -y java-1.8.0-openjdk-devel.x86_64

Go in application directory:
  
    cd spring-music

Build the app
  
    ./gradlew clean assemble

Create a service with the plan

    cf create-service elephantsql turtle spring-db

List out the local services

    cf services

Bind the app with db service

    cf bind-service spring-music spring-db
    cf restage spring-music

