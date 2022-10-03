pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
		cd ~/msp/e2e-playwright
                pytest ~/msp/e2e-playwright/tests/fco/test_save_extended_data.py --headless False --slow_motion 0 --workers 1 --tests-per-worker 1 --reruns 0 --pve 49
            }
        }
    }
}
