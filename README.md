# Ansible Role : install_figurine

[![CI](https://github.com/glillico/ansible-role-install_figurine/workflows/CI/badge.svg)](https://github.com/glillico/ansible-role-install_figurine/actions?query=workflow%3ACI)

Download and install the figurine binary.

## Requirements

None

## Role Variables

### defaults/main.yml

|Variable|Default Values|Description|
|---|---|---|
|inf_url|https://github.com/arsham/figurine/releases/download|Download URL|
|inf_version|1.3.0|Version|
|inf_platform|linux|OS Platform|
|inf_arch|arm64|CPU Architechure|
|inf_path|/usr/local/bin|Path to extract file into|

By using the above variable values the playbook would download the file `https://github.com/arsham/figurine/releases/download/v1.3.0/figurine_linux_arm64_v1.3.0.tar.gz` and extract it into `/usr/local/bin`.

## Dependencies

None

## Example Playbook

    - hosts: servers
      roles:
         - glillico.install_figurine

## License

MIT

## Author Information

Created in 2024 by Graham Lillico.
