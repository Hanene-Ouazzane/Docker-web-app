node {
    checkout scm

    docker.withRegistry('hub.docker.com', 'dockerHub') {

        def customImage = docker.build("pushautomation:${env.BUILD_ID}")

        /* Push the container to the custom Registry */
        customImage.push()
    }
}
