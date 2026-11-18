pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Compilando el código fuente...'
                // Ejemplo Node.js: sh 'npm install && npm run build'
                // Ejemplo Java Maven: sh 'mvn clean package -DskipTests'
                // Ejemplo Python: sh 'pip install -r requirements.txt'
            }
        }

        stage('Test') {
            steps {
                echo 'Ejecutando pruebas unitarias...'
                // Ejemplo Node.js: sh 'npm test'
                // Ejemplo Java Maven: sh 'mvn test'
                // Ejemplo Python: sh 'pytest'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Desplegando la aplicación en el entorno de prueba...'
                // Ejemplo Docker: sh 'docker compose up -d --build'
                // Ejemplo script propio: sh './deploy-staging.sh'
            }
        }
    }

    post {
        success {
            echo 'Pipeline completado con éxito.'
        }
        failure {
            echo 'El pipeline falló. Revisa los logs de la etapa con error.'
        }
    }
}
