stage('push image'){
    docker.withRegistry('https://registry.hub.docker.com', 'dockerHub'){
        app.push("${ENV.BUILD_NUMBER}")
        app.push("latest")
            }
            }
           
