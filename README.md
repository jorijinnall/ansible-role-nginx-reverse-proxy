# Reverse Proxy

## Introduction to this role
Install Nginx as a reverse proxy.
The role also use letsencrypt to automatically create and renew certificates for the websites given

## Configuration
Check defaults/main.yml to see the list of variables to use

The following variables are here to list the websites to create and where to redirect the flow
```yaml
sites:
  - site_name: test.foo.bar
    site_port: 8080
    site_host: 127.0.0.1
    site_enabled: true
