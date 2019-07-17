node {
stage ('Scm Checkout'){
git "https://github.com/vinaykurakula07/JavaWebCalculator"
}  
stage ('compile-package'){
  // getting Maven Home path
  def mvnhome = tool name: 'mvn', type: 'maven'  
  sh "${mvnhome}/bin/mvn package"
}
  stage ('Email Notifaication'){
  
    mail bcc: 'vinaykurakula07@gmail.com', body: '''Hi Welcome to Jenkins Gmail Notification
Thanks
Vinay''', cc: '', from: '', replyTo: '', subject: '', to: 'vinay.devops93@gmail.com'
  }
}

