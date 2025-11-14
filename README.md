<!-- START doctoc generated TOC please keep comment here to allow auto update -->
<!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->
**Table of Contents**  *generated with [DocToc](https://github.com/thlorenz/doctoc)*

- [ansible-netplan](#ansible-netplan)
  - [Requirements](#requirements)
  - [Role Variables](#role-variables)
  - [Dependencies](#dependencies)
  - [Example Playbook](#example-playbook)
  - [License](#license)
  - [Author Information](#author-information)

<!-- END doctoc generated TOC please keep comment here to allow auto update -->

# ansible-netplan

An [Ansible](https://www.ansible.com) role to manage [Netplan](https://netplan.io)

## Requirements

## Role Variables

See [defaults/main.yml](defaults/main.yml) for the full list. Key options:

- `netplan_config_file`: Destination rendered Netplan YAML path.
- `netplan_configuration`: Data structure rendered into the Netplan config. Leave empty to skip rendering.
- `netplan_remove_existing`: When true (default) existing Netplan YAML files (except the target file) are pruned before provisioning.
- `netplan_debug_configs`: When true, logs the discovered existing Netplan files for troubleshooting. Defaults to `false` to avoid extra output and speed up runs.

## Dependencies

## Example Playbook

## Testing

- Install Molecule’s runtime deps (Python `molecule[docker]`, `yamllint`, `ansible-lint`, Docker Engine).
- From the repo root run `molecule test` to execute the full create → converge → verify → destroy cycle.
- Use `molecule converge`/`molecule verify` when iterating to shorten feedback loops.

## License

MIT

## Author Information

Larry Smith Jr.

-   [EverythingShouldBeVirtual](http://everythingshouldbevirtual.com)
-   [@mrlesmithjr](https://www.twitter.com/mrlesmithjr)
-   <mailto:mrlesmithjr@gmail.com>
