FROM openjdk:11 AS BUILD_IMAGE
RUN apt update && apt install maven -y && apt install git -y
<<<<<<< HEAD
RUN git clone -b docker https://github.com/devopshydclub/vprofile-project.git
RUN cd vprofile-project && mvn install

FROM tomcat:9-jre11
RUN rm -rf /usr/local/tomcat/webapps/*
COPY --from=BUILD_IMAGE vprofile-project/target/vprofile-v2.war /usr/local/tomcat/webapps/ROOT.war
EXPOSE 8080
CMD ["catalina.sh", "run"]
=======
RUN git clone --branch docker https://github.com/devopshydclub/vprofile-project.git
RUN cd vprofile-project && mvn install

FROM tomcat:9-jre11

RUN rm -rf /usr/local/tomcat/webapps/*
LABEL "Project"="Vprofile"
LABEL "AUthor"="SSgaikwad"
COPY --from=BUILD_IMAGE vprofile-project/target/vprofile-v2.war /usr/local/tomcat/webapps/ROOT.war
EXPOSE 8080
CMD ["catalina.sh","run"]
>>>>>>> d176436e5e6a6fcab5b9256d30138d59c97f94ab
