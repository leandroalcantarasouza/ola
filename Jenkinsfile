node {
    stage "Build Image"
        //sh "docker run -p 8081:8080 -d --name teste apresentacao-backend:java"
        checkout scm
        def customImage = docker.build("apresentacao-backend:java")
        customImage.inside() {
            sh "java -version"
        }
}