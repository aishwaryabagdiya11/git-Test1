pipeline {
    agent any
    environment{
        a="velocity"
    }

    stages {
        stage('printing variable') {
            steps {
                
            sh '''
                echo "this is user define global variable$(a)"
                '''
            }
			
            stage('stage level variable') {
                environment{
                    b="pune"
                }
            steps {
                
            sh '''
                echo "this is user define global variable$(b)"
                '''
            
        }
    }
}
}
}

