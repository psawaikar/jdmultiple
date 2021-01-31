node {
    def frontend
    def backend

    stage('Checkout') {
        checkout scm
    }

    stage('Dev') {
        //echo "Hello World"
        frontend = docker.build('psawaikar/jdmultiple_frontend:3.0', "--no-cache -f ${env.WORKSPACE}/frontend/Dockerfile .")
        backend = docker.build('psawaikar/jdmultiple_backend:3.0', "--no-cache -f ${env.WORKSPACE}/backend/Dockerfile.qa .")
        //def DB = docker.build("my-image:${env.BUILD_ID}","-f ${env.WORKSPACE}/db/Dockerfile .")

        //**** Unit Testing of each docker image goes here -- ADD LATER

        //docker.image('alpine:latest').inside {
        //sh 'echo Hello World!'
        //}
    }

    stage('BAT') {
        //**** BAT tests to be run here -- ADD LATER
        //app1.push()

        //docker.withRegistry('https://registry.hub.docker.com/', 'psawaikar-DockerHub') {

        //    app1.push('2.0')
        //}
    }

    stage('QA') {
        //**** QA tests to be run here -- ADD LATER
        echo "QA Stage - TBD LATER"
    }





}