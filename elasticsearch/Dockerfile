ARG ELASTIC_VERSION

# https://www.docker.elastic.co/
FROM docker.elastic.co/elasticsearch/elasticsearch:${ELASTIC_VERSION}

# Add your elasticsearch plugins setup here
# Example: RUN elasticsearch-plugin install analysis-icu

env ELK_VERSION=8.7.0
# Add your elasticsearch plugins setup here
# Example: RUN elasticsearch-plugin install analysis-icu
RUN elasticsearch-plugin install --batch https://github.com/medcl/elasticsearch-analysis-ik/releases/download/v${ELK_VERSION}/elasticsearch-analysis-ik-${ELK_VERSION}.zip 
