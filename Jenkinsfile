pipeline {
    agent any

    stages {
        stage('Clonar repositorio') {
            steps {
                git 'https://github.com/prespik/node-hello-world.git'
            }
        }

        stage('Instalar dependencias') {
            steps {
                bat 'npm install'
            }
        }

        stage('Ejecutar aplicación') {
            steps {
                bat 'npm start &'
                echo 'Aplicación iniciada. Puedes agregar pruebas si lo deseas.'
            }
        }
    }
}
