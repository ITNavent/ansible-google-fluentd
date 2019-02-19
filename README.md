# Ansible Google Fluentd

Ansible role that installs Google Logging Agent (Fluentd)

## Variables

+ Active configurations. syslog and syslog_endpoint enabled by default.
```yaml
google_fluent_active_configs:           
  - syslog
  - syslog_endpoint
```
+ Copies this files to the configurations folder. They are not enabled by default, so you must add them to the ```google_fluent_active_configs``` list.
```yaml
google_fluent_custom_config_files: []
```
+ Copies this templates to the configurations folder. They are not enabled by default, so you must add them to the ```google_fluent_active_configs``` list.
```yaml
google_fluent_custom_config_templates: []
```

+ Adds this folder as a configuration folder. Every *.conf file in this folder will be included.
```yaml
google_fluent_custom_config_folder: ''
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