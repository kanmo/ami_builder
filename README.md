# AMIBuilder

Language installed AMI builder by Packer and Ansible.  
Languages are Elixir, Erlang, Ruby.

# Setup
Packer and Ansible instllation required.  
AWS shared credentials file required.  

1. Packer

```
brew install packer
```

If you don't use Mac, Homebrew, please read [this](https://www.packer.io/docs/install/index.html)

2. Ansible

```
brew install ansible
```

If you don't use Mac, Homebrew, please read [this](http://docs.ansible.com/ansible/latest/intro_installation.html)

3. AWS shared credentials file
Please read [this](https://docs.aws.amazon.com/sdk-for-go/v1/developer-guide/configuring-sdk.html#creating-the-credentials-file)

# Example
case Elixir.

```
PROFILE=default TYPE=elixir packer build packer/build.json
```

- PROFILE is AWS credential's profile name.
- TYPE is language to install.
