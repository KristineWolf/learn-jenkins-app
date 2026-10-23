pipeline {
    agent any
    
    stages {
        stage('Build') {
            steps {
                cleanWs()
                sh '''
                echo "Building a new laptop..."
                echo $BUILD_FILE_NAME
                mkdir -p build
                touch build/$BUILD_FILE_NAME
                echo "MainBoard" >> build/$BUILD_FILE_NAME
                cat build/$BUILD_FILE_NAME
                '''
            }
        }
    }
}
