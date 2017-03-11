node {
        stage("Main build") {
            checkout scm

            docker.image('maven:3.3.3-jdk-8').inside {

              stage("Install Bundler") {
		git url: 'https://github.com/TTFHW/jenkins_pipeline_java_maven.git'
                sh "mvn -B clean install"
              }

           }

        }

}
