# ldap

- to run the local ldap server: docker run -p 389:389 -p 636:636 --name my-openldap-container --detach osixia/openldap:1.2.4

- to find the details of the users and verify the ldap server: docker exec my-openldap-container ldapsearch -x -H ldap://localhost -b dc=example,dc=org -D "cn=admin,dc=example,dc=org" -w admin

 - demo user credentials:
   - username: admin
   - password: admin
