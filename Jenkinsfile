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
echo "Stage Build"
}
}
stage("Deploy") {
steps {
sh "docker run -d -p 4000:80 flask-docker"
}
}
}
}