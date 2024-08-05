pipeline {
  agent any
  stages {
    stage('myStage'){
      steps {
        httpRequest (console LogResponseBody: true,
          contentType: 'APPLICATION_JSON",
          httpMode: 'POST',
          requestBody: command,
          url: "http://localhost:8088/startTests",
          validResponseCodes: '200')
      }
    }
    stage('Build') {
      steps {
        httpRequest (consoleLogResponseBody: true,
          contentType: 'APPLICATION_JSON",
          httpMode: 'POST',
          requestBody: command,
          url: "http://localhost:8088/startTests",
          validResponseCodes: '200')
      }
    }
  }
}
