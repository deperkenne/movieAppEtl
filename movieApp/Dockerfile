
FROM apache/airflow:3.0.1-python3.11
USER root

RUN apt-get update && \
    apt-get install -y gcc  python3-dev  openjdk-17-jdk && \
    apt-get clean

ENV JAVA_HOME /usr/lib/jvm/java-17-openjdk-amd64

USER airflow

RUN  pip install --upgrade pip
RUN pip install apache-airflow-providers-apache-spark pyspark
