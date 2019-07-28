# WordPress Develop Docksal
A Docker-based WordPress development environment built using Docksal.

## Default Environment
- PHP 7.2
- Apache 2.4
- MySQL 5.6.

These can be customized using a `.docsal-local.env` file.

The NGINX configuration is already included in the repo to make for easily switching between Apache/NGINX without any additional setup required.

## Tools
- WPCLI
- Xdebug
- PHPMyAdmin
- Mailhog

## Custom Commands
The full range of Docksal `fin` commands are available. Check out [the documentation](https://docs.docksal.io/fin/fin-help/) for usage, or run `fin help`.

In addition, there are a few helpful custom commands included.

Usage: `fin <command> <options>`

- `init` - Intialize the project. Clones `wordpress-develop` using Git, installs all dependencies, builds WordPress, and sets up PHPUnit testing configuration.
- `install-wp` - Allows you to just reinstall WordPress DB and config in the event of a project reset, so you don't have to do the full `init` again.
- `patch` - Applys a patch directly from Trac
- `phpunit` - Run PHPUnit tests without having to install PHPUnit on your machine, or SSH into a VM
- `xdebug` - Toggle Xdebug on and off

## Installation
1. Install Docksal - https://docs.docksal.io/getting-started/setup/
2. Clone this repo
```bash
git clone git@github.com:earnjam/wpcoredocksal.git
```

3. Switch into the repository directory
```bash
cd wpcoredocksal
```
4. Initialize the project
```bash
fin init
```
