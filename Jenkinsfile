node('master') {
    stage("scm"){checkout([$class: 'GitSCM', branches: [[name: '*/master']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[credentialsId: 'dbd5a9e0-dfc1-4edd-97f4-b24a3fd2c3e5', url: 'https://github.com/vamsichitipothu/learn_maven_build.git']]])
    }
    stage("build"){ sh'mvn install'}
}
