# Ansible Role for Certbot

## Description

This Ansible role is designed for installing and configuring Certbot for managing Let's Encrypt SSL/TLS certificates on Nginx servers. It includes tasks for installing Certbot and its Nginx plugin, generating certificates for specified domains, and setting up automatic certificate renewal.

## Features

- Installing Certbot and its Nginx plugin.
- Generating SSL certificates for domains specified.
- Auto-renewal setup for SSL certificates.

## Requirements

- Ansible 2.14 or higher.
- A Debian or Ubuntu-based system with Nginx installed.

## Role Variables

The role uses the following variables which can be defined in the playbook:

- `certbot_email`: The email address used for registration and recovery with Let's Encrypt.
- `acme_domains`: A list of domains for which to generate SSL certificates.

Example `defaults/main.yml`:

```yaml
---
# defaults file for certbot

certbot_email: "kk573@axes.ru"
acme_domains: []
