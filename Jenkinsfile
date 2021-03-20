pipeline {
  agent any

  stages {
    stage ('Installing npm dependencies') {
      steps {
        sh 'export PATH=/usr/local/bin  npm install'
        // Bat 'npm install'
      }
    }

    stage ('Run Unit Test') {
      steps {
        sh 'export PATH=/usr/local/bin npm run test'
      }
    }
  }
}

// Build - execute shell


// #!/bin/bash
// export PATH=$PATH:/usr/local/bin
// echo "libarary path"
// echo $PATH
// echo "${GIT_BRANCH}"
// BRANCH_NAME=${GIT_BRANCH}
// echo "$BRANCH_NAME"
// echo "installing..."
// npm install || exit 1

// if [ "$BRANCH_NAME" == "origin/develop" ]
// then
// echo "building development..."
// ng build || exit 1
// ls
// sudo azcopy make "https://anguarjenkinsapp.blob.core.windows.net/angularjenkinsapp?sv=2020-02-10&ss=bfqt&srt=sco&sp=rwdlacupx&se=2021-03-18T18:55:59Z&st=2021-03-18T10:55:59Z&spr=https&sig=Wzt%2B2hSSQJ8%2F5Pjwm5HYlJ7zFBXG2o7s8n0s%2BVGmFNY%3D"
// sudo azcopy copy 'dist/**' 'https://anguarjenkinsapp.blob.core.windows.net/angularjenkinsapp?sv=2020-02-10&ss=bfqt&srt=sco&sp=rwdlacupx&se=2021-03-18T18:55:59Z&st=2021-03-18T10:55:59Z&spr=https&sig=Wzt%2B2hSSQJ8%2F5Pjwm5HYlJ7zFBXG2o7s8n0s%2BVGmFNY%3D' --recursive
// fi

// if [ "$BRANCH_NAME" == "origin/staging" ]
// then
// echo "building staging..."
// ng build --configuration=staging || exit 1
// ls
// sudo ./azcopy copy 'dist/**' '<SAS URL STAGING>/$web?<REST QUERY PARAMS>' --recursive
// fi