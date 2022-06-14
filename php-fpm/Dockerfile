# FROMでベースのイメージを指定する。
FROM php:7.4-fpm


# RUNはコマンドを実行する。
#pdoインストール
RUN docker-php-ext-install pdo_mysql

#composerインストール
RUN curl -sS https://getcomposer.org/installer | php
RUN mv composer.phar /usr/local/bin/composer

#gitインストール
RUN apt-get update
RUN apt-get install -y git

RUN apt-get install -y zip unzip