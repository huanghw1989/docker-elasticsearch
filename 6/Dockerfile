FROM docker.elastic.co/elasticsearch/elasticsearch:6.8.8
LABEL maintainer="huanghongwu <huanghongwu@perfectcode.tech>"


RUN /usr/share/elasticsearch/bin/elasticsearch-plugin install --batch analysis-ik && \
    /usr/share/elasticsearch/bin/elasticsearch-plugin install --batch analysis-pinyin && \
    /usr/share/elasticsearch/bin/elasticsearch-plugin install --batch analysis-icu && \
    /usr/share/elasticsearch/bin/elasticsearch-plugin install --batch analysis-smartcn
