pipeline {
    agent any

    stages{
        // Integracion Continua
        stage('Instalar Dependencias'){
            steps{
                sh 'npm install'
            }
        }

        stage('Compilacion del APP'){
            steps{
                sh 'npm run build'
            }
        }

        stage('Mostrar Archivos'){
            steps{
                sh 'ls -la'
            }
        }

        // Despliegue
        stage('Desliegue de la Aplicacion'){
            steps{
                sh 'cp dist/democlase06/* /usr/ucreativa/romell2/'
            }
        }
    }
}
