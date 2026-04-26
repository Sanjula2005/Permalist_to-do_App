for c1 (only maven no jenkinsfile) and c2:

maven.yml
name: Java CI/CD Pipeline
on:
  push:
    branches:
      - master
jobs:
  build:
    runs-on: windows-latest
    env:
      FORCE_JAVASCRIPT_ACTIONS_TO_NODE24: true
    steps:
      - uses: actions/checkout@v4
      - name: Setup Java
        uses: actions/setup-java@v4
        with:
          distribution: temurin
          java-version: '17'
      - name: Build using Maven
        run: mvn clean install
        working-directory: demo

















c2:
pipeline {
    agent any

    tools {
        maven 'Maven3'
    }

    stages {

        stage('Checkout') {
            steps {
                git 'https://github.com/SinchanaNagendra/maven_waste.git'
            }
        }

        stage('Build') {
            steps {
                dir('demo') {
                    bat 'mvn clean install'
                }
            }
        }

        stage('Test') {
            steps {
                dir('demo') {
                    bat 'mvn test'
                }
            }
        }
    }
}



go to: https://api.slack.com/apps







