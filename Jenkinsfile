node('linux') {
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
//	stage ('post-clean') {
//		cleanWs()
//	}
}
