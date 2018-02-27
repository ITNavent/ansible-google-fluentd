# Ansible Google Fluentd

Ansible role that installs Google Logging Agent (Fluentd)

# Variables

```yaml
google_fluent_extra_configs_path: ""    # Adds this directory to fluentd lookup places for configurations. Undefined by default
google_fluent_active_configs:           # Active configurations. syslog and syslog_endpoint enabled by default.
  - syslog
  - syslog_endpoint
```

## Available configuration

Values for ```google_fluent_active_configs``` must come from this list:
- apache
- cassandra
- chef
- forward
- gitlab
- jenkins
- jetty
- joomla
- magento
- mediawiki
- memcached
- mongodb
- mysql
- nginx
- postgresql
- puppet
- puppet-enterprise
- rabbitmq
- redis
- redmine
- salt
- solr
- sugarcrm
- syslog
- syslog_endpoint
- tomcat
- zookeeper