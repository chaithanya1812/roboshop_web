FROM nginx
ADD https://roboshop-artifacts.s3.amazonaws.com/frontend.zip  /tmp/
RUN apt-get update && apt-get install unzip -y
RUN  rm -rf /usr/share/nginx/html/* && \
     rm -rf /etc/nginx/nginx.cong &&  \
    rm -rf /etc/nginx/conf.d/default.conf && \
    unzip /tmp/frontend.zip -d /usr/share/nginx/html/

# COPY roboshop.conf /etc/nginx/nginx.conf  # Iam doing at run-time configfuration as volume..
