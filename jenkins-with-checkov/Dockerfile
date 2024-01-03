FROM jenkins/jenkins:jdk21
WORKDIR /tmp
RUN curl "https://awscli.amazonaws.com/awscli-exe-linux-x86_64.zip" -o "awscliv2.zip"
RUN unzip awscliv2.zip
USER root
RUN ./aws/install
RUN apt update
RUN apt install python3-full -y
RUN apt install pip -y
RUN pip install checkov --break-system-packages