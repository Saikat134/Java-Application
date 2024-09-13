pipeline{
    agent any
    stages{
        stage("Git checkout"){
            steps{
                echo "This is for a Git Checkout"
            }
        stage("stage 2"){
            input{
                message 'Is it okay to continue?'
                ok 'Yes,we should'
            }
            steps{
                echo "This is for a Stage 2"
            }    
            
        }
    }
    post{
        always{
            echo "========always========"
        }
        success{
            echo "========pipeline executed successfully ========"
        }
        failure{
            echo "========pipeline execution failed========"
        }
    }
}
}