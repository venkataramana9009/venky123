node {

    checkout scm

    docker.withRegistry('https://registry.hub.docker.com', 'hanudocker') {

        def customImage = docker.build("hanumantharao1986/dockerimageramana$BUILD_NUMBER")

        /* Push the container to the custom Registry */
        customImage.push()
    }
}
