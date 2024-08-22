pipeline{
    agent any
    stages {
        stage ("seq-1") {
            steps {
                sleep 10
            }
        }
        stage ("parallel-stages"){
            parallel {
                stage ("stage-1") {
                    steps {
                        sleep 10
                        echo "this is stage-1"
                    }
                }
                stage ("stage-2"){
                    steps{
                        sleep 10
                        echo "this is stage-2"
                    }
                }
                stage ("stage-3") {
                    steps {
                        sleep 10
                        echo "this is stage-3"
                    }
                }
                
            }
        }
      stage ("seq-2")  {
          steps {
              sleep 10
          }
      }
    }
}
