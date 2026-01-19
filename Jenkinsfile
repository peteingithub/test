pipeline {
  agent any
  stages {
    stage('Stage 1: Running the Pre Build Commands') { 
      steps {
        echo 'Stage 1 commands ...'
      }
    }
    stage('Stage 2: Build a new Container Image') { 
      steps {
        echo 'Stage 2 commands ...'
      }
    }
    stage('Stage 3: Pushing the Image to the Registry') { 
      steps {
        echo 'Stage 3 commands ...'
      }
    }
    stage('Stage 4: Creating a new App') { 
      steps {
        echo 'Stage 4 commands ...'
      }
    }
    stage('Stage 5: Scanning the Image with SUSE Security') { 
      steps {
        echo 'Stage 5 commands ...'
                neuvector nameOfVulnerabilityToExemptFour: '',
        nameOfVulnerabilityToExemptOne: '', 
        nameOfVulnerabilityToExemptThree: '', 
        nameOfVulnerabilityToExemptTwo: '', 
        nameOfVulnerabilityToFailFour: '', 
        nameOfVulnerabilityToFailOne: '', 
        nameOfVulnerabilityToFailThree: '', 
        nameOfVulnerabilityToFailTwo: '', 
        numberOfHighSeverityToFail: '10', 
        numberOfMediumSeverityToFail: '10', 
        registrySelection: 'rmt', 
        repository: "registry.suse.com/bci/bci-base", 
        scanLayers: true, 
        tag: "15.7"
      }
    }
    stage('Stage 6: Deploying the Application to the Develpment Cluster') { 
      steps {
        echo 'Stage 6 commands ...'
      }
    }
  }
}
