FROM nginx:alpine

COPY --from=itezaz/letscode:frontend /frontend/build/ /usr/share/nginx/html

RUN rm /etc/nginx/conf.d/default.conf
COPY nginx.conf /etc/nginx/conf.d
EXPOSE 80
CMD ["nginx", "-g", "daemon off;"]
