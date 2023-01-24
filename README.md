# ngnix-ssl-docker-localhost
This project is a website built using Nginx and served via a local development environment using Docker.
The website is secured using SSL certificates generated using mkcert, which allows for HTTPS connections on localhost.
This project can be used as a starting point for developing and testing web applications in a secure and isolated environment on a local machine.

1. installing mkcert using brew (mac user) - brew install mkcert
2. getting SSL certificate for choosen domain using mkcert, I used "Dor.com" -  mkcert Dor.com
   - The certificate will be created at "./**yourDomain**.pem" and the key at "./**yourDomain**-key.pem"
3. move the certificate and the key to "cert" folder
4. run - docker-compose up -d