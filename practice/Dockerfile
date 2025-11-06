FROM almalinux:9

ARG version

RUN dnf install nginx -y
RUN rm -rf /usr/share/nginx/html/index.html 

COPY index.html /usr/share/nginx/html/index.html

CMD ["nginx" , "-g" , "daemon off;"]

#direct url from the internet and copying to location
ADD https://chatgpt.com/c/68fc6984-1964-8323-8a49-dfdc5df68507  /usr/share/nginx/html/index.html 
#untaring the file and copying to location
ADD myfiles.tar.gz /app/ 

LABEL COURSE="devops"\
      TRAINER="SIVA"\
      HRS="2hrs"

EXPOSE 80 

ENV COURSE="DEVOPS"\
    TRAINER="SIVA"\
    HRS="2HRS" 
    

CMD ["ping"]
ENTRYPOINT ["google.com"]

RUN useradd jaggu
USER jaggu

ARG trainer="jaggu"
ENV tariner=$trainer
