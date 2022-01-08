pipeline {
  agent any
  
  environment {
    DEVENV = 'https://dev76270.service-now.com'
    CREDENTIALS = 'bf228170-dfd6-4771-b372-8dc5fd5ad2ca'
  }
  stages {
    stage('activate-plugin') {
      steps {
        snActivatePlugin(
          url: "${DEVENV}",
          credentialsId: "${CREDENTIALS}",
          pluginId: 'sn_role_builder')
      }
    }
  }
}
