parallel linux: {
    node('linux') {
        checkout scm
        sh 'python test_runner.py'
    }
},
windows: {
    node('mac') {
        checkout scm
        sh 'python test_runner.py'
    }
}