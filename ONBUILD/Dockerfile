# almalinux is exactly same as Redhat image, but completely free
FROM almalinux:9
RUN dnf install nginx -y
RUN rm -rf /usr/share/nginx/html/index.html
#This instruction run when someone use this image
ONBUILD COPY index.html /usr/share/nginx/html/index.html
CMD ["nginx","-g","daemon off;"]