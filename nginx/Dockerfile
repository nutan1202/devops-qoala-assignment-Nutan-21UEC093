# # FROM nginx:latests
# # COPY nginix.conf /etc/nginx/nginx.conf
# # COPY ./html /usr/share/nginx/htmll

# EXPOSE "eighty"
# CMD ["nginx", "-g", "daemon of;"]

#spelling of latest corrected
FROM nginx:latest
COPY nginx.conf /etc/nginx/nginx.conf
#i was encountering error as html file was not there so commented it
# COPY ./html /usr/share/nginx/html

#correction for syntax for writing the port number
EXPOSE 80
CMD ["nginx", "-g", "daemon off;"]
