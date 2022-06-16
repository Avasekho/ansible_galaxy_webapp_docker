FROM maven:3.8.5-jdk-11
RUN apt update
WORKDIR /tmp/
RUN git clone https://github.com/boxfuse/boxfuse-sample-java-war-hello.git
WORKDIR /tmp/boxfuse-sample-java-war-hello/
RUN mvn package
WORKDIR /tmp/boxfuse-sample-java-war-hello/target/
RUN mkdir /shared_folder/
RUN mv hello-1.0.war /shared_folder/