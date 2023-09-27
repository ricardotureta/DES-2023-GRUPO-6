
# Click nbfs://nbhost/SystemFileSystem/Templates/Licenses/license-default.txt to change this license
# Click nbfs://nbhost/SystemFileSystem/Templates/Other/Dockerfile to edit this template

FROM tomcat:9.0
RUN mvn clean install
CMD ["mvn", "clean", "install"]
COPY ./target/shopping-cart-0.0.1-SNAPSHOT.war /usr/local/tomcat/webapps/app.war
CMD mvn clean install && mvn clean install -U
EXPOSE 8080
CMD ["catalina.sh", "run"]