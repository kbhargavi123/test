pipeline {
    agent any

     
    stages {
        stage('checkout scm') {
            steps {
                cleanWs()
                git 'https://github.com/kbhargavi123/test.git'
                echo 'checkedout scm'
            }
        }
        stage('tar') {
            steps {
               
               sh '''
                 tar -cvf water/xyz.tar *
                 echo "files are compressed"
                 tar -xvf water/xyz.tar
                 '''
               
             
            }
        }
    }
}
