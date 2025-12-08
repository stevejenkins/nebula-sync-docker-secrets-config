# nebula-sync-docker-secrets-config
My Docker compose and secrets configuration files for synchonizing Pi-holes via Nebula-Sync






cd /opt/nebula-sync
mkdir secrets
cd secrets
 nano primary.txt
 http://123.123.123.123:8089|xxxxxxxxxxxxxxxxxxxxxxxxxxxx=

 Dont forget = at the send of the string

 nano replicas.txt
http://124.124.124.124:80|xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx,http://125.125.125.125:80|xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx=
