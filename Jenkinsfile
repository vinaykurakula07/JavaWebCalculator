node {
stage ('Scm Checkout'){
git "https://github.com/vinaykurakula07/JavaWebCalculator"
}
  
stage ('compile-package'){
  // getting Maven Home path
  
def mvnhome = tool name: 'mvn', type: 'maven'
  
  sh "${mvnhome}/bin/mvn package"
}
}

