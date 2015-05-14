FROM nginx:latest
MAINTAINER Victor Bocharsky <bocharsky.bw@gmail.com>

# Change Nginx config here...
RUN rm /etc/nginx/conf.d/default.conf
ADD ./default.conf /etc/nginx/conf.d/

CMD ["nginx", "-g", "daemon off;"]
