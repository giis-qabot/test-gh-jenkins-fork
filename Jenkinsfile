/* Change from fork
Para configurar invocacion desde github a jenkins sin usar el GitHub plugin que devuelve el status
y permite acceder a jenkins desde GitHub:
En jenkins:
- Instalar Multibranch Scan Webhook Trigger
En el multibranch job: 
- Branch source Git (no GitHub)
- Scan multibranch pipeline triggers: scan by webhook e indicar un token
En el repo GitHub:
- webhook con payload: https://in4test.lsi.uniovi.es/jengis/multibranch-webhook-trigger/invoke?token=TOKEN
*/
pipeline {
  agent {label 'slave-x1'}
  options { disableConcurrentBuilds() }
  stages {
    stage('test') {
        steps{
            sh 'ls -la'
        }
    }
  }
}
