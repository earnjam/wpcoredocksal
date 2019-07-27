FROM docksal/cli:2-php7.2

USER root

# Add PHPUnit
RUN wget https://phar.phpunit.de/phpunit-7.5.phar \
	&& chmod +x phpunit-7.5.phar \
	&& sudo mv phpunit-7.5.phar /usr/local/bin/phpunit
