FROM phpmyadmin/phpmyadmin:fpm

RUN echo '' >> /usr/local/etc/php/conf.d/php-phpmyadmin.ini \
 && echo '[PHP]' >> /usr/local/etc/php/conf.d/php-phpmyadmin.ini \
 && echo 'post_max_size = 2G' >> /usr/local/etc/php/conf.d/php-phpmyadmin.ini \
 && echo 'upload_max_filesize = 2G' >> /usr/local/etc/php/conf.d/php-phpmyadmin.ini

ENV PMA_ARBITRARY=1 \
  PMA_HOST=laravel_local \
  PMA_PORT=3306 \
  PMA_USER=phper \
  PMA_PASSWORD=secret
