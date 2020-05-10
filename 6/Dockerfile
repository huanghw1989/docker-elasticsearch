FROM docker.elastic.co/elasticsearch/elasticsearch:6.8.8
LABEL maintainer="huanghongwu <huanghongwu@perfectcode.tech>"


RUN /usr/share/elasticsearch/bin/elasticsearch-plugin install --batch analysis-icu && \
    /usr/share/elasticsearch/bin/elasticsearch-plugin install --batch analysis-smartcn && \
    /usr/share/elasticsearch/bin/elasticsearch-plugin install --batch analysis-phonetic && \
    /usr/share/elasticsearch/bin/elasticsearch-plugin install --batch mapper-size && \
    /usr/share/elasticsearch/bin/elasticsearch-plugin install --batch mapper-murmur3 && \
    /usr/share/elasticsearch/bin/elasticsearch-plugin install --batch mapper-annotated-text && \
    # For 6.x
    /usr/share/elasticsearch/bin/elasticsearch-plugin install --batch discovery-file && \
    # other plugin
    /usr/share/elasticsearch/bin/elasticsearch-plugin install --batch https://github.com/medcl/elasticsearch-analysis-ik/releases/download/v6.8.8/elasticsearch-analysis-ik-6.8.8.zip
