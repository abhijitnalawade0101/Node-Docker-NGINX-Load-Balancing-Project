## Project Features
- **Node.js Application**: A simple server (`server.js`) responding to HTTP requests.
- **Dockerized Environment**:  
  - `Dockerfile` for Node.js app  
  - `docker-compose.yaml` for multi-container orchestration
- **NGINX Configuration**:  
  - HTTP (`nginx.conf.http_load_bal_code`)  
  - HTTPS (`nginx.conf.https_code`)  
  - Self-signed SSL certificates for HTTPS testing

  Build and start Docker containers
  
    `docker compose up --build`

    `docker compose up --build -d`

  ## In Nginx:
         mkdir /nginx-certs cd /nginx-certs
         Run this command
         openssl req -x509 -nodes -days 365 -newkey rsa:2048 -keyout nginx-selfsigned.key -out nginx-selfsigned.crt 
         it will create two key public key and private add your code 

         Then you need to find nginx.conf for your system and paste the code that require to run like if you http code use http templte or if you want secure connection then https conf templte paste in your code
         start nginx

## Commands used in the tutorial

    start nginx
    
    nginx
    get options
    
    nginx -h
    restart nginx
    
    nginx -s reload

    stop nginx
    
    nginx -s stop

## secure connection through nginx https
<img width="1880" height="886" alt="Screenshot 2026-02-16 123048" src="https://github.com/user-attachments/assets/9233780a-7069-4243-bcef-62ebd54c46b0" />



         
