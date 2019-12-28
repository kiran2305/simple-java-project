 node{
      stage('git checkout'){
           git credentialsId: '5d50c5dd-a745-444f-bf4a-16aaf1ebcb32', url: 'https://github.com/kiran2305/simple-java-project.git'
      }
        stage('build'){
            def maven= tool name: 'maven3.6.0', type: 'maven'
            def mavencmd= "${maven}/bin/mvn"
            sh "${mavencmd} compile package"
      }

  }

  
