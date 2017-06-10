:set paste

def dlist='/boot'
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
          sh "echo '${dlist}'"
          println "${myparam}"
      }
}
