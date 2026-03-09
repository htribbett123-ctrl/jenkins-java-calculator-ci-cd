# jenkins-java-calculator-ci-cd
# Jenkins CI/CD Pipeline – Java Calculator Project

![Build Status](https://img.shields.io/badge/Jenkins-Build%20Passing-brightgreen)
![Java](https://img.shields.io/badge/Java-17-blue)
![Maven](https://img.shields.io/badge/Maven-Build%20Automation-C71A36)
![JUnit](https://img.shields.io/badge/Tests-JUnit5-success)
![Coverage](https://img.shields.io/badge/Coverage-JaCoCo-yellow)

# Jenkins CI/CD Pipeline — Java Calculator Project

This project contains a simple Java Calculator application built with Maven and tested using JUnit 5. It is designed for use in a Jenkins CI/CD pipeline to demonstrate automated builds, testing, and code coverage reporting.


## CI/CD Pipeline Overview

This project is used in a Jenkins CI/CD pipeline that:
- Pulls code from GitHub
- Runs Maven build and tests
- Publishes JUnit test results

- [1;36m                         ┌────────────────────────────────┐[0m
[1;36m                         │          Developer              │[0m
[1;36m                         │   (Commit / Push to GitHub)     │[0m
[1;36m                         └──────────────────┬──────────────┘[0m
                                               │
                                               ▼
[1;34m                         ┌────────────────────────────────┐[0m
[1;34m                         │          GitHub Repo            │[0m
[1;34m                         │ jenkins-java-calculator-ci-cd   │[0m
[1;34m                         └──────────────────┬──────────────┘[0m
                                               │
                                   [1;33m(SCM Polling / Webhook)[0m
                                               │
                                               ▼
[1;32m     ┌──────────────────────────────────────────────────────────────────────┐[0m
[1;32m     │                               Jenkins                                │[0m
[1;32m     │                     Continuous Integration Server                     │[0m
[1;32m     └──────────────┬───────────────────────────────┬──────────────────────┘[0m
                      │                               │
                      ▼                               ▼
[1;35m       ┌──────────────────────────┐     ┌──────────────────────────────┐[0m
[1;35m       │        Maven Build        │     │         JUnit Testing        │[0m
[1;35m       │   mvn clean test package  │     │   Surefire Test Execution    │[0m
[1;35m       └──────────────┬───────────┘     └──────────────┬──────────────┘[0m
                        │                                │
                        ▼                                ▼
[1;33m       ┌──────────────────────────┐     ┌──────────────────────────────┐[0m
[1;33m       │     Compiled Classes     │     │     XML Test Reports         │[0m
[1;33m       │      target/classes      │     │ target/surefire-reports/*.xml│[0m
[1;33m       └──────────────┬───────────┘     └──────────────┬──────────────┘[0m
                        │                                │
                        ▼                                ▼
[1;32m     ┌──────────────────────────────────────────────────────────────────────┐[0m
[1;32m     │                        Jenkins Test Reporting                         │[0m
[1;32m     │     ✔ Build Status  ✔ Test Summary  ✔ Historical Trends               │[0m
[1;32m     └──────────────────────────────────────────────────────────────────────┘[0m


## Features
- Java Calculator with basic operations (add, subtract, multiply, divide)
- JUnit 5 test suite
- Maven build configuration
- Clean folder structure for CI/CD pipelines


## CI/CD Ready
This project is optimized for Jenkins:
- GitHub integration
- Maven build steps
- JUnit test reporting

## Project Structure

- src/main/java/com/example/calculator/Calculator.java
src/test/java/com/example/calculator/CalculatorTest.java
pom.xml


![Build Status](https://img.shields.io/badge/Jenkins-Build%20Passing-brightgreen)
