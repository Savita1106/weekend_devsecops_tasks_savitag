node
{
  stage("1.creating the files")
  echo "checking the files"
  sh "ls -a"
  sh "mkdir -p test-folder"
  sh "touch test-folder/test.sh"

  stage("2.install some packages")
  sh "sudo yum update -y"
  sh "sudo yum install httpd -y"
  sh "sudo systemctl restart httpd"
  sh "sudo systemctl enable httpd"
  sh "rpm -qa |grep httpd"
  sh "ps -auxx |grep httpd"
}
