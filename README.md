<p align="center">
  <a href="https://roots.io/bedrock/">
    <img alt="Bedrock" src="https://cdn.roots.io/app/uploads/logo-bedrock.svg" height="100">
  </a>
</p>


<p align="center">
  <strong>A modern WordPress stack with Docker</strong>
</p>

<p align="center">
  <a href="https://roots.io/"><strong><code>Website</code></strong></a> &nbsp;&nbsp; <a href="https://docs.roots.io/bedrock/master/installation/"><strong><code>Documentation</code></strong></a> &nbsp;&nbsp; <a href="https://github.com/roots/bedrock/releases"><strong><code>Releases</code></strong></a> &nbsp;&nbsp; <a href="https://discourse.roots.io/"><strong><code>Support</code></strong></a>
</p>

## Overview

Bedrock is a modern WordPress stack that helps you get started with the best development tools and project structure.

Much of the philosophy behind Bedrock is inspired by the [Twelve-Factor App](http://12factor.net/) methodology including
the [WordPress specific version](https://roots.io/twelve-factor-wordpress/).

### Contains

- Bedrock
- Docker
- Apache

### Servers
- [http://localhost/](http://localhost/) - wordpress
- [http://localhost:8080/](http://localhost:8080/) - phpmyadmin
- [http://localhost/wp/](http://localhost/wp/) - wordpress admin
- [http://localhost:8025/](http://localhost:8025/) - MailHog

## Requirements

- PHP >= 7.4
- Docker
- Composer - [Install](https://getcomposer.org/doc/00-intro.md#installation-linux-unix-osx)

## Installation

1. Clone repo
2. Run `composer isntall`
3. (Optional) Update environment variables in the `.env` file. Wrap values that may contain non-alphanumeric characters with
   quotes, or they may be incorrectly parsed.
4. (Optional) Update `docker` folder or `docker-compose.yml`
5. (Optional)  Add theme(s) in `web/app/themes/` as you would for a normal WordPress site
6. Run `docker-compose up`
7. Access WordPress admin at `https://example.com/wp/wp-admin/`