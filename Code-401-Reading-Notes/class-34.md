# class_34
## Configuring Django Settings
### Managing Django Settings: Issues
* Different environments. Usually, you have several environments: local, dev, ci, qa, staging, production, etc
* Sensitive data. You have SECRET_KEY in each Django project. 
* Sharing settings between team members. You need a general approach to eliminate human error when working with the settings
* Django settings are a Python code. This is a curse and a blessing at the same time. 

### Setting Configuration: Different Approaches
There is no built-in universal way to configure Django settings without hardcoding them.

### Separate settings file for each environment
This is an extension of the previous approach. It allows you to keep all configurations in VCS and to share default settings between developers.

#### Pros:
All environments are in VCS.<br>
It’s easy to share settings between developers.
#### Cons:
* You need to find a way to handle secret passwords and tokens.
* “Inheritance” of settings can be hard to trace and maintain.
#### Environment variables
To solve the issue with sensitive data, you can use environment variables.


## SSH
SSH, or Secure Shell, is a remote administration protocol that allows users to control and modify their remote servers over the Internet.

It provides a mechanism for authenticating a remote user, transferring inputs from the client to the host, and relaying the output back to the client.

### How Does SSH Work
The SSH command consists of 3 distinct parts:

    ssh {user}@{host}
* ssh: instructs your system that you want to open an encrypted (Secure Shell Connection)
* user: the account you want to access
* host: refers to the computer you want to access.This can be an IP Address or a domain name
