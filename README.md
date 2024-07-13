

## Stages
- create instance with jenkins:
    <p>
    sudo apt update<br>
    sudo apt install fontconfig openjdk-17-jre<br>
    java -version
      <br>
      <br>
    sudo wget -O /usr/share/keyrings/jenkins-keyring.asc \<br>
    https://pkg.jenkins.io/debian-stable/jenkins.io-2023.key<br>
    echo deb [signed-by=/usr/share/keyrings/jenkins-keyring.asc] \<br>
    https://pkg.jenkins.io/debian-stable binary/ | sudo tee \<br>
    /etc/apt/sources.list.d/jenkins.list > /dev/null<br>
    sudo apt-get update<br>
    sudo apt-get install jenkins<br>
    ---> then proceed with the first installation of jenkins <---
    </p>
- prebuild configurations:
  add this plugin:
  <img width="869" alt="image" src="https://github.com/IftachZilcaPaz/jenkins_aws_git/assets/151572520/e9165d99-0229-43ce-a46a-3524a251af80"><br>
  then:<br>
  <img width="366" alt="image" src="https://github.com/IftachZilcaPaz/jenkins_aws_git/assets/151572520/8599234b-1a95-4bd8-9759-d656223abdac"><br>
  then:<br>
  <img width="1245" alt="image" src="https://github.com/IftachZilcaPaz/jenkins_aws_git/assets/151572520/c8b3b2b8-c0c4-4fdb-a9c1-8bbafb50be08">
  <img width="1262" alt="image" src="https://github.com/IftachZilcaPaz/jenkins_aws_git/assets/151572520/641aed78-c50f-46be-a470-6e91e9534116">




  
- build new proj in jenkins:
  <img width="970" alt="image" src="https://github.com/IftachZilcaPaz/jenkins_aws_git/assets/151572520/bba81560-2c56-4d8c-89e6-ebe88d370f20"><br>
  put here the git repo https url:<br>
  <img width="1022" alt="image" src="https://github.com/IftachZilcaPaz/jenkins_aws_git/assets/151572520/0000b2d9-46df-44ae-8b9f-d807c6c4a2f4"><br>
  make sure that the branch is main or master, and check the "GitHub hook trigger for GITScm polling"<br>
  <img width="1089" alt="image" src="https://github.com/IftachZilcaPaz/jenkins_aws_git/assets/151572520/734fb9f4-65d3-4a42-8cdc-f97100284b6f"><br>
  then build execute shell:<br>
  <img width="1000" alt="image" src="https://github.com/IftachZilcaPaz/jenkins_aws_git/assets/151572520/defae5de-2591-4c51-b68e-f0e6082f5cb4"><br>
  and another one:<br>
  <img width="1008" alt="image" src="https://github.com/IftachZilcaPaz/jenkins_aws_git/assets/151572520/310c91ca-8ebd-4fb8-ab5f-83740cc4ea96"><br>


- github webhook:
  <img width="1137" alt="image" src="https://github.com/IftachZilcaPaz/jenkins_aws_git/assets/151572520/ee4790d3-a2a9-432f-b522-58311d0b1561"><br>
  add webhook<br>
  <img width="785" alt="image" src="https://github.com/IftachZilcaPaz/jenkins_aws_git/assets/151572520/733a4035-cc8f-4fc4-8f96-53012c67f4ac"><br>
  select this:<br>
  <img width="271" alt="image" src="https://github.com/IftachZilcaPaz/jenkins_aws_git/assets/151572520/d582a5db-236d-4155-b7cc-15058fd21d99"><br>
  and this:<br>
  <img width="605" alt="image" src="https://github.com/IftachZilcaPaz/jenkins_aws_git/assets/151572520/9db03558-38c2-4726-9f8d-9682ab7224b3"><br>
  then save, now when we change somethins and push or we change it in the web it will trigger the jenkins








  
