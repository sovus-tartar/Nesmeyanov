
# How to create ssh-key?
* run powershell as administrator
* run '''ssh-keygen -t ed25519 -C "email.email.com"'''

# How to add key to github account?
* go to 'settings -> SSH and GPG keys -> new ssh key'
* open your ssh-key file in text editor and copy its contains
* paste its contains into field for key
* push 'add ssh key'

# How to add private key to ssh-agent?
* run '''Get-Service ssh-agent | Set-Service -StartupType Manual'''
* run '''Start-Service ssh-agent'''
* run '''Get-Service ssh-agent'''
* run '''ssh-add ~\.ssh\id_ed25519'''

# How to clone repository?
* run '''git clone git@github.com:username/repository.git'''
