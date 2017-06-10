#!/usr/bin/env groovy

def dlist=''
def myparam='/boot'
println dlist

node ('master') {
    stage ('Stage_1') {
          if(isUnix()) {
              println ('IS_UNIX = TRUE')
          }
      }
     stage ('Stage_2') {
        sh 'cd /; ls -l; ls -d'
      }
      stage ('Stage_3') {
          println "Branch"
          sh "echo '${dlist}'"
          println "${myparam}"
      }
}
