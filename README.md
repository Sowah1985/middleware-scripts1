#!/bin/bash

Author: Nancy
Date: 02/23/23
Description: Sonarqube installation


su - sonar

sudo yum update -y

sudo yum install java-11-openjdk-devel -y

sudo yum install java-11-openjdk -y

cd /opt

sudo yum install wget -y

sudo wget https:binaries.sonarsorce.com/Distruation

