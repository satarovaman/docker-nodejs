node {
    checkout scm

    docker.withRegistry('https://registry.hub.docker.com', 'docker-amake') {

        def customImage = docker.build("satarovaman/nodejs-app")

        /* Push the container to the custom Registry */
        customImage.push()
    }
}
