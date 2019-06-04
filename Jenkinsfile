
pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
                "prebuild": "npm run build:clean",
                "build": "cross-env NODE_ENV=production webpack --config internals/webpack/webpack.prod.babel.js --color -p --progress --hide-modules --display-optimization-bailout",
                "build:clean": "rimraf ./build",
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}