# https://github.com/elastic/logstash-docker
FROM docker.elastic.co/logstash/logstash-oss:6.2.4

# Add your logstash plugins setup here
# Example: RUN logstash-plugin install logstash-filter-json
# chmod 777 /usr/share/logstash/pipeline/logstash.conf


RUN set -x \
    && chown -R logstash.logstash /usr/share/logstash \
	&& chmod 777 /usr/share/logstash/data


COPY pipeline/logstash.conf /usr/share/logstash/pipeline/
