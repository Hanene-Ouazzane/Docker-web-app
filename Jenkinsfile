node {
    checkout scm

    docker.withRegistry('index.docker.io', 'dockerHub') {

        def customImage = docker.build("pushautomation:${env.BUILD_ID}")

        /* Push the container to the custom Registry */
        customImage.push()
    }
}
