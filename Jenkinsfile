abcd = ['a','b','c','d']
node('master') {
        stage('testing loop') {
                echo_all (abcd)
        }
}
def echo_all(list) {
        list.each {item ->
                sh "This is ${item}"
        }
}
