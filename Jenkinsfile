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
stage("Deploy") {
steps {
sh "docker run -p 4000:80 flask-docker"
}
}
}
}