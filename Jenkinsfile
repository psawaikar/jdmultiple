node {
    def frontend
    def backend

    stage('Checkout') {
        checkout scm
    }

    stage('Dev') {
        //echo "Hello World"
        frontend = docker.build('psawaikar/jdmultiple_frontend:1.0', "-f ${env.WORKSPACE}/frontend/Dockerfile .")
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