# show-ansible-secrets

Show encrypted secrets in an ansible vars file.

## Dependency

This script uses `yq`, a python util to parse yaml files.

## Installation

You must install `yq` with `pip3 install yq` for this script to work.

Then just set the right permissions: `chmod a+x show_secrets`

## Usage

- `show_secrets [options] \<vars_file>`
- `show_secrets -h|--help`

## Options

| Option                                                  | Description                                                 |
|---------------------------------------------------------|-------------------------------------------------------------|
| `-h`, `--help`                                          | Display this help                                           |
| `-k <key>`, `--key=<key>`                               | Decrypt only for the given secret name (repeatable)         |
| `-p <password_file>`, `--password-file=<password_file>` | Specify the password file (if not defined in `ansible.cfg`) |
| `-v`, `--version`                                       | Show version                                                |
