wrboyce.dotfiles-zsh
====================

[![Build Status](https://travis-ci.org/wrboyce/ansible-dotfiles-zsh.svg)](https://travis-ci.org/wrboyce/ansible-dotfiles-zsh)

Configure zsh using [oh-my-zsh](https://github.com/robbyrussell/oh-my-zsh) and oh-my-zsh/custom repo.

Requirements
------------

Depends on the `user_home` and `user_usernames` variables being set.

Role Variables
--------------

Custom repo defaults to `https://github.com/{{ user_username }}/oh-my-zsh-custom.git`, variable `user_username` or
`zsh_omz_custom_repo` must be set.

Example Playbook
----------------

    - hosts: workstations
      roles:
         - wrboyce.dotfiles-zsh

License
-------

Apache 2.0
