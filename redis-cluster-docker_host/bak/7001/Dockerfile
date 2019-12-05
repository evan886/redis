FROM redis:5.0.2
COPY redis.conf /usr/local/etc/redis/redis.conf
RUN ln -sf /usr/share/zoneinfo/Asia/Shanghai /etc/localtime
RUN echo 'Asia/Shanghai' >/etc/timezone
RUN chmod 777 /usr/local/etc/redis/redis.conf

EXPOSE 7001
EXPOSE 17001

CMD [ "redis-server", "/usr/local/etc/redis/redis.conf" ]conf
