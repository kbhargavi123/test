pipeline {
    agent any

     
    stages {
        stage('checkout scm') {
            steps {
                git branch: 'main', url: 'https://github.com/kbhargavi123/test.git'
                echo 'checkedout scm'
            }
        }
        stage('tar') {
            steps {
               
               sh '''
                 tar -zcvf xyz.tar.gz test
                 tar -zxvf water/xyz.tar.gz
                 '''
               
             
            }
        }
    }
}
