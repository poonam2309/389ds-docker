# 389ds-docker

docker run -t --name demo-389ds -p 127.0.0.1:389:389  -e "DIRSRV_ADMIN_USERNAME=Directory Manager,DIRSRV_ADMIN_PASSWORD=admin@123, DIRSRV_MANAGER_PASSWORD=admin@123, DIRSRV_SUFFIX=dc=lic,dc=com" fabric8/389ds:latest

docker ps -a
docker cp annuity-sheet/ldap-users2.ldif cbc108098267:/tmp
docker exec -it cbc108098267 /bin/bash 

ldapadd  -h localhost -D "cn=Directory Manager" -wadmin@123 -f /tmp/ldap-users2.ldif 


