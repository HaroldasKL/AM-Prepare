FROM wordpress:6.6.2

RUN curl -O https://raw.githubusercontent.com/wp-cli/builds/gh-pages/phar/wp-cli.phar \
    && chmod +x wp-cli.phar \
    && mv wp-cli.phar /usr/local/bin/wp

COPY ./wp-automatic /var/www/html/wp-content/plugins/wp-automatic
# COPY ./disable-update-notifications /var/www/html/wp-content/plugins/disable-update-notifications

# wp plugin activate wp-automatic --allow-root --path=/var/www/html/;
# wp plugin activate disable-update-notifications --allow-root --path=/var/www/html/;
