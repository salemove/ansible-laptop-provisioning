You will need to install brew first

You will need to install ansible second

```bash
brew install ansible
```

Go ahead and execute the following to install all packages you will need, you can also install recommended packages in addtion to the required packages

```bash
# Install required packages
ansible-playbook glia.yaml

# Or you can execute the following to install required and recommended packages
ansible-playbook --tags=recommended glia.yaml
```

You may be prompted for a password, enter your sudo password

# Installing other packages

There are a few other packages you can install in the ./other_packages path, to install those, execute the following:

```bash
ansible-playbook other_packages/oh-my-zsh.yaml
```

You can install multiple packages by appending multiple playbooks

```bash
ansible-playbook glia.yaml other_packages/oh-my-zsh.yaml