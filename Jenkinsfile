node {
    checkout scm

    docker.withRegistry('https://registry.hub.docker.com', 'credentials-id') {

        def customImage = docker.build("satarovaman/nodejs-app")

        /* Push the container to the custom Registry */
        customImage.push()
    }
}
