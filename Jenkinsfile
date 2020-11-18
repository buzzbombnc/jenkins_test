pipeline {
    agent any
    options {
        timestamps()
    }
    stages {
        stage('folder1') {
            when {
                changeset "folder1/**"
            }
            steps {
                build 'folder1'
            }
        }
        stage('folder2') {
            when {
                changeset "folder2/**"
            }
            steps {
                build 'folder2'
            }
        }
    }
}
