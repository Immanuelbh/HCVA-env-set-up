ARG ELK_VERSION

# https://www.docker.elastic.co/
FROM docker.elastic.co/elasticsearch/elasticsearch:${ELK_VERSION}

# Add your elasticsearch plugins setup here
# ARG needs to be redeclared after FROM statement
# https://stackoverflow.com/a/56748289/6432241
ARG ELK_VERSION
RUN elasticsearch-plugin install --batch "https://github.com/Immanuelbh/elasticsearch-analysis-hebrew/releases/download/elasticsearch-analysis-hebrew-${ELK_VERSION}/elasticsearch-analysis-hebrew-${ELK_VERSION}.zip"
