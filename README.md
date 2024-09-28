# basicdockerwithnginx
This repos consist of simple index.html page and a docker file
   
    
    #Base Image
    FROM nginx:alpine
    # MAINTAINER of the Dockerfile
    MAINTAINER Pramesh <pramesh@oxpanmicrosys.com>
    
    #copy index.html file to /usr/share/nginx/html/
    COPY index.html /usr/share/nginx/html/
    
    #Expose Nginx port
    EXPOSE 80
    
    #Start NginxService
    CMD ["nginx","-g","daemon off;"]

