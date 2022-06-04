# Training engineer

## Homework 03 - justanotherhelloworld

### Instructions

В репозитории GitHub найти проекты на Java, собрать их с помощью системы сборки Maven.
Получить артефакты сборки JAR, WAR файлы.
WAR артефакты запустить в контейнере сервлетов Apache Tomcat.

### Tiny log

    # apt update
    # apt install -y maven tomcat9 curl
    # ss -nlpt | grep 8080
    ...
    # git clone https://github.com/daticahealth/java-tomcat-maven-example
    # cd java-tomcat-maven-example
    # mvn package
    ...
    # cp target/java-tomcat-maven-example.war /var/lib/tomcat9/webapps/
    # curl http://127.0.0.1:8080/java-tomcat-maven-example/ 
    <html>
    <body>
    <h2>Hello World!</h2>
    </body>
    </html>
    # rm /var/lib/tomcat9/webapps/java-tomcat-maven-example.war
    # nano src/main/webapp/index.jsp
    ...
    # mvn clean
    ...
    # mvn package
    ...
    # cp target/java-tomcat-maven-example.war /var/lib/tomcat9/webapps/
    curl http://127.0.0.1:8080/java-tomcat-maven-example/
    <html>
    <body>
    <h2>DEVOPS NEVER GIVE UP</h2>
    </body>
    </html>


### Screenshot

![a little proof](https://github.com/mitropolitippolit/training_engineer/raw/master/homework03/screenshot.png)
