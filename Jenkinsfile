pipeline {
		agent {
			label "main"
		}
			stages {
				stage("23Q1"){
				steps {
					sh "cd/mnt/docker-deploy"
					sh "git checkout 23Q1"
					sh "docker run -itd 80:80 --name 23Q1 httpd"
					sh "docker exec -it 23Q1 bash"
					sh "cd htdocs"
					sh "chmod 777 index.html"
					sh "docker cp index.html 23Q1:/usr/local/apache2/htdocs"
				}
				
				}
			
	stages {
				stage ("23Q2") {
				
				steps{
          sh "cd/mnt/docker-deploy"
					sh "git checkout 23Q2"
					sh "docker run -itd 80:80 --name 23Q2 httpd"
					sh "docker exec -it 23Q2 bash"
					sh "cd htdocs"
					sh "chmod 777 index.html"
					sh "docker cp index.html 23Q2:/usr/local/apache2/htdocs"

          
        }
				
				
				} 
			}
			
			}
