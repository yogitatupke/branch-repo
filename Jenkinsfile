pipeline {
		agent any 
			stages {
				stage("23Q2"){
				steps {
					//sh "cd /mnt"//
					//sh "cd git clone https://github.com/yogitatupke/branch-repo.git "//
					//sh "cd .."//
					//sh "systemctl start docker"//
					sh "systemctl status docker"
					//sh "systemctl enable docker"//
					//sh "docker pull httpd"//
					sh "docker stop 23Q2"
					sh "docker rm 23Q2"
					sh "docker system prune -a -f"
					sh "docker run -itdp 8000:80 --name 23Q2 httpd"
					sh "docker cp index.html 23Q2:/usr/local/apache2/htdocs"
					sh "docker exec 23Q2 chmod -R 777 /usr/local/apache2/"
     }
			
	
    
			}
}
}
					

					
