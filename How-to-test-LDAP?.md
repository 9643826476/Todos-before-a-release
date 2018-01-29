# Testing LDAP with Docker

Clone [administration](https://github.com/owncloud/administration) repo and run `ldap-testing/start.sh` to start a LDAP server

```
git clone https://github.com/owncloud/administration
administration/ldap-testing/start.sh
```
## Fill the LDAP instance with a zombie army

Run `administration/ldap-testing/batchCreateUsers.php` from the same folder in the `administration` repo.

```
cd administration/ldap-testing/
php batchCreateUsers.php
```

## Fill the LDAP instance with multiple zombie armies (groups) 

Edit `administration/ldap-testing/config.php` with desired parameters

Run `administration/ldap-testing/batchCreateUsersInGroups.php` from the same folder in the `administration` repo.

```
cd administration/ldap-testing/
gedit config.php
php batchCreateUsersInGroups.php
```

## Setup user_ldap

Tested config:

* Server: `localhost`, Port: gets autodetected (if not click the "detect port" button)
* User DN: `cn=admin,dc=owncloud,dc=com`
* Password: `admin`
* Base DN: `dc=owncloud,dc=com` (gets autodetected once you have filled Server, Port, User DN and Password)
* User Filter: `inetOrgPerson` as object class should be fine (default value)
* Login Filter: `LDAP Username` works (default value)
* Group Filter: not needed
* Advanced -> Directory Settings -> User Display Name Field: `displayName` (camelCase ;))
* Expert -> UUID Attribute for Users: `uid`
* Advanced -> Directory Settings -> Group-Member association: `memberUid` (without memberof) or `member` (with memberof)

# How to login as LDAP user
Every zombie has a user name (e.g. zombie294), which you can use to login on ownCloud. As password use the username. You can find all usernames with PHPLDAPAdmin

# Happy Testing