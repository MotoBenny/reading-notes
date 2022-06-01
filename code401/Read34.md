## [Django settings best practices](https://djangostars.com/blog/configuring-django-settings-best-practices/)

Djangos settings are python code, this is both cool and not very cool, since it can create conflicts and sometimes has quite tricky logic. 

Local settings files, are generally names `settings_local.py`

Although it is easy to lose your settings between enviroments with this method.

Separate sttings files for each enviroment
with this method its easy to share settings between developers, 

enviroment cariables
great for sensitive data.


### [SSH](https://www.hostinger.com/tutorials/ssh-tutorial-how-does-ssh-work)

Secure Shell Protocol - remote administration allowing users remote access to their servers over the internet 

Mac and linux machines natively support SSH, a windows machine will need to use a external client like PuTTY

#### **Symmetric Encryption**

Symmetric encryption is a form of encryption where a **secret key** is used for both encryption and decryption of a message by both the client and the host. Effectively, anyone possessing the key can decrypt the message being transferred.

#### **Asymmetric Encryption**

Unlike symmetrical encryption, asymmetrical encryption uses two separate keys for encryption and decryption. These two keys are known as the **public key** and the **private key**. Together, both these keys form a **public-private key pair**.

#### **Hashing**

One-way hashing is another form of cryptography used in Secure Shell Connections. One-way-hash functions differ from the above two forms of encryption in the sense that they are never meant to be decrypted. They generate a unique value of a fixed length for each input that shows no clear trend which can be exploited. This makes them practically impossible to reverse.