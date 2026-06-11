FROM almalinux:9
RUN dnf install nginx -y
RUN rm -rf /usr/share/nginx/html/index.html
ADD https://raw.githubusercontent.com/Pavankotha9550/terraform-roboshop-dev-module/refs/heads/main/30-module-category/ec2.tf /usr/share/nginx/html/index.html
RUN chmod +r https://raw.githubusercontent.com/Pavankotha9550/terraform-roboshop-dev-module/refs/heads/main/30-module-category/ec2.tf
CMD ["nginx" , "-g" , "daemon off;"]