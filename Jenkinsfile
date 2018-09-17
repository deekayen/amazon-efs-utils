node('use1ddbuild04||use1ddbuild05') {
	stage ('pre-clean') {
		cleanWs()
	}
	stage ('clone scm') {
		git 'https://github.com/aws/efs-utils.git'
	}
	stage ('build') {
        sh '''#!/bin/bash

make rpm'''
    }
	stage ('post-clean') {
		cleanWs()
	}
}
