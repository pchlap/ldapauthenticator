# ldapauthenticator

Fork of Simple LDAP Authenticator Plugin for JupyterHub. This has been customized 
to attempt PAM Authentication before proceeding with LDAP Authentication.

An optional prefix for the username passed to the system can be configured in the 
case of LDAP authentication. The purpose of this is to deal with LDAP users 
consisting of only numbers.

## Installation ##

You can install it from pip with:

```
pip install https://github.com/pchlap/ldapauthenticator/archive/master.zip
```

## Usage ##

See the original repository for usage and configuration: [Simple LDAP 
Authenticator Plugin for JupyterHub](https://github.com/jupyterhub/ldapauthenticator)


### Optional configuration ###

#### `LDAPAuthenticator.system_user_prefix` ####

Prefix the returned username with the given value.

```python
c.LDAPAuthenticator.system_user_prefix = 'u'
```
