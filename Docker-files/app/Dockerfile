
FROM openjdk:11 AS BUILD_IMAGE
RUN apt update && apt install maven -y && apt install git -y
RUN git clone -b docker https://github.com/devopshydclub/vprofile-project.git
RUN cd vprofile-project && mvn install 



