# Ansible Role: `aisbergg.rmate`

This Ansible role installs the [rmate](https://github.com/aurora/rmate) script. Rmate allows to edit files on a remote server using an editor like TextMate, Visual Studio Code or Atom.

## Requirements

None.

## Role Variables

| Variable | Default | Comments |
|----------|---------|----------|
| `rmate_repository` | `https://github.com/aurora/rmate.git` | Repository to install the rmate script from. |
| `rmate_version` | `latest` | The script version to install. The value can be either a specific value (e.g. '1.0.2') or 'latest'. |
| `rmate_aliases` | `['rcode']` | Aliases for the executable. |

## Example Playbook

```yaml
- hosts: all
  vars:
    rmate_version: latest
    rmate_aliases:
      - rcode

  roles:
    - aisbergg.rmate
```

## Dependencies

None.

## License

MIT

## Author Information

Andre Lehmann (aisberg@posteo.de)
