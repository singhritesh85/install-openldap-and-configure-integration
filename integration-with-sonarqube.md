vim /opt/sonarqube/conf/sonar.properties             


sonar.security.realm=LDAP
ldap.url=ldap://172.31.1.253:389                                           
ldap.bindDn=cn=ldapadm,dc=singhritesh85,dc=com
ldap.bindPassword=unix
ldap.user.baseDn=ou=People,dc=singhritesh85,dc=com
ldap.user.request=(&(objectClass=inetOrgPerson)(uid={login}))
ldap.user.realNameAttribute=cn
ldap.user.emailAttribute=mail
ldap.group.baseDn=ou=Group,dc=singhritesh85,dc=com
ldap.group.request=(&(objectClass=groupOfUniqueNames)(uniqueMember={dn}))
sonar.log.level=DEBUG



Now Restart the Sonarqube.
