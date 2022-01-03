<h1 align="center">
  Ansible Role for <a href="https://www.zsh.org/">zsh</a> & <a href="https://github.com/zsh-users/antigen/">antigen</a>
</h1>

<p>
  <a href="./LICENSE" target="_blank">
    <img alt="License: MIT" src="https://img.shields.io/badge/License-MIT-green.svg?style=for-the-badge" />
  </a>
</p>

> This repo contains a zero-configuration Linux-distro agnostic Ansible role that installs [zsh](https://www.zsh.org/) + [antigen plugin manager](https://github.com/zsh-users/antigen).

## Requirements

- No additional requirements.

- ⚠️ Note: the role assumes that you already have `~/.zshrc` file in place with antigen config on target host machine.

  Example `.zshrc` file content:

  ```zsh
  source ~/.antigen/antigen.zsh
  antigen use oh-my-zsh
  antigen bundle git
  antigen theme bira
  antigen apply
  ```

## Example Ansible Playbook

```yaml
- hosts: 127.0.0.1
  roles:
    - role: ansible-role-zsh-antigen
      vars:
        zsh_set_as_default_shell: true
```

## Author

👤 **Alexander Danilenko**

* Website: https://danilenko.in
* Github: [@alexander-danilenko](https://github.com/alexander-danilenko)
* LinkedIn: [@alexander-danilenko](https://linkedin.com/in/alexander-danilenko)

## 🤝 Contributing

Contributions, issues and feature requests are welcome!<br />Feel free to check [issues page](https://github.com/alexander-danilenko/ansible-role-zsh-antigen/issues). 

## Show your support

Give a ⭐️ if this project helped you!

## 📝 License

Copyright © 2022 [Alexander Danilenko](https://github.com/alexander-danilenko).<br />
This project is [MIT](./LICENSE) licensed.

***
_This README was generated with ❤️ by [readme-md-generator](https://github.com/kefranabg/readme-md-generator)_