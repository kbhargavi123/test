pipeline {
    agent any

     
    stages {
        stage('checkout scm') {
            steps {
                git 'https://github.com/kbhargavi123/test.git'
                echo 'checkedout scm'
            }
        }
        stage('tar') {
            steps {
               
               sh '''
                 tar -zcvf water/xyz.tar.gz *
                 echo "files are compressed"
                 tar -zxvf water/xyz.tar.gz
                 '''
               
             
            }
        }
    }
}
