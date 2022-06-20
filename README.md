# MKAMATERA

Command line interface to [kamatera](https://www.kamatera.com/) cloud service.

## Dependencies

- [sh-hutil](https://github.com/harkaitz/sh-hutil).
- [curl](https://curl.se/).
- [jq](https://stedolan.github.io/jq/).

## Configuring.

You must set the following environment variables.

- KAMATERA_API_CLIENT_ID
- KAMATERA_API_SECRET
- KAMATERA_SERVER_PASS : Put here a command that prints the password to use in servers.
- KAMATERA_IMG : Image to use in server, ie EU:6000C29278ba3895e04246ad2f1d8388

## Help

mkamatera

    Usage: mkamatera ...
    
    ... show                  : Show configuration.
    ... ls                    : List servers.
    ... ls-o OPTS...          : List options.
        | billing cpu         |
        | datacenter image    |
        | network ram traffic |
    ... create NAME           : Create machine.
    ... tasks                 : See recent commands.
    ... uuid   NAME|UUID      : Get UUID of a machine.
    ... billing [MONTH] [YEAR]: Print usage info.
    ... password              : Get main password.
    ... p-hosts               : Print /etc/hosts for kamatera servers.
    ... p-ssh_config          : Print /etc/ssh/ssh_config for kamatera servers.
    ... u-locals              : Update /etc/hosts, /etc/ssh/ssh_config.
    
    ... NAME|UUID power on|off|restart : Set power state.
    ... NAME|UUID ipaddr               : Get IP address.
    ... NAME|UUID rename NAME          : Rename machine.
    ... NAME|UUID attach               : Open terminal.
    ... NAME|UUID resetpass            : Change password.
    ... NAME|UUID sshkey               : Upload ssh key.

## Collaborating

For making bug reports, feature requests and donations visit
one of the following links:

1. [gemini://harkadev.com/oss/](gemini://harkadev.com/oss/)
2. [https://harkadev.com/oss/](https://harkadev.com/oss/)

