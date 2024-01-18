FROM schoolofdevops/carts-maven:3.9

WORKDIR /opt/carts/

COPY ./carts .

RUN mvn package -D skipTests

RUN mv target/carts.jar /run/ && rm -rf *

EXPOSE 80

CMD 


