//import jenkins.model.Jenkins
//import jenkins.model.*

def dlist='/boot'
def myparam='/boot'
println dlist

node ('master') {
//if (getBinding().hasVariable("myparam")) {
//        println getProperty("myparam")
//    }
//    node {sh 'env'}
    env.SNAPSHOT='TRUE'
    println get.env
    println 'SNAPSHOT = '. SNAPSHOT

    stage ('Stage_1') {
        if(isUnix()) {
            println ('IS_UNIX = TRUE')
        }
    }
   stage ('Stage_2') {
       new File("/").eachFile() { file->  
           println file.getName()  
       }
   }
    stage ('Stage_3') {
        sh "echo '${dlist}'"
        println "${myparam}"
    }
}