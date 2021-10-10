# ansible_role_xfce

[![badge](https://img.shields.io/badge/Xfce-Desktop-green?logo=xfce)](https://xfce.org/)

This role installs sddm as login window and Xfce as desktop manager thus usign much less ressources than gnome desktop.

## Variables

Variables with examples:

```yml
# set to yes in order to set the graphical target as default
# this is not really idempotent
xfce_target_graphical_default: true

# set to your default target name if you want to unset graphical target
# e.g. 'multi-user' if the default should be 'multi-user.target'
xfce_target_undo_default: "multi-user"
```

## Example Usage

```yml
roles:
  - ansible-role-xfce
```

## Acknowledgements

- many thanks to the old CentOS forum: <https://forums.centos.org/viewtopic.php?t=72433>

## License

MIT
