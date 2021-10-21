pipeline{
    agent any
    tools {
        nodejs 'node'
    }
    options{
        timeout(time:10, unit:'MINUTES')
    }
    stages{
        stage('Instalación de dependencias'){
            steps{
                sh 'npm install'
            }
        }
        stage('ns doctor'){
            steps{
                sh 'ns doctor android'
            }
        }
        stage('Generación APK'){
            steps{
                sh 'ns build android'
            }
        }
        stage('Pruebas unitarias'){
            steps{
                sh 'echo "Pruebas unitarias (en construcción)"'
            }
        }
        stage('Pruebas funcionales'){
            steps{
                sh 'echo "Pruebas funcionales (en construcción)"'
            }
        }
        stage('Pruebas de carga'){
            steps{
                sh 'echo "Pruebas de carga (en construcción)"'
            }
        }
        stage('SauceLab'){
            steps{
                sh 'echo "SauceLab (en construcción)"'
            }
        }
        stage('Despliegue en Google Play'){
            steps{
                sh 'echo "Despliegue en Google Play (en construcción)"'
            }
        }
    }
}