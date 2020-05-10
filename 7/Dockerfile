FROM docker.elastic.co/elasticsearch/elasticsearch:7.6.2
LABEL maintainer="huanghongwu <huanghongwu@perfectcode.tech>"


RUN /usr/share/elasticsearch/bin/elasticsearch-plugin install --batch analysis-icu && \
    /usr/share/elasticsearch/bin/elasticsearch-plugin install --batch analysis-smartcn && \
    /usr/share/elasticsearch/bin/elasticsearch-plugin install --batch analysis-phonetic && \
    /usr/share/elasticsearch/bin/elasticsearch-plugin install --batch mapper-size && \
    /usr/share/elasticsearch/bin/elasticsearch-plugin install --batch mapper-murmur3 && \
    /usr/share/elasticsearch/bin/elasticsearch-plugin install --batch mapper-annotated-text && \
    # other plugin
    /usr/share/elasticsearch/bin/elasticsearch-plugin install --batch https://github.com/medcl/elasticsearch-analysis-ik/releases/download/v7.6.2/elasticsearch-analysis-ik-7.6.2.zip