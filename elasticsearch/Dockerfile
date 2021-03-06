ARG ELK_VERSION

# https://www.docker.elastic.co/
FROM docker.elastic.co/elasticsearch/elasticsearch:${ELK_VERSION}

# Add your elasticsearch plugins setup here
RUN elasticsearch-plugin install --batch https://github.com/Immanuelbh/plugin-test-release/releases/download/v${ELK_VERSION}/elasticsearch-analysis-hebrew-${ELK_VERSION}.zip
