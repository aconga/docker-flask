pipeline {
agent any
stages {
stage("Checkout") {
steps {
echo 'Checkout'
}
}
stage("Docker build") {
steps {
sh "docker build -t flask-docker ."
}
}
}
}