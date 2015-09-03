FROM haron/vim

MAINTAINER Dmitry Bespalov <bespalovdn@gmail.com>

USER root

WORKDIR /home/dev
RUN rm -rf .vim*
COPY config /home/dev/
RUN chown -R dev:dev .

USER dev

CMD vim
