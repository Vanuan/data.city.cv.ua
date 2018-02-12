
    docker-compose up



    
TODO

Create admin user:

paster --plugin=ckan user add admin email=admin@example.com -c /etc/ckan/ckan.ini
paster --plugin=ckan sysadmin add admin -c /etc/ckan/ckan.ini 



1. create datastore database
2. set datastore db permissions
    paster --plugin=ckan datastore set-permissions -c /etc/ckan/ckan.ini
3. configure datapusher
4. apply config to production
5. resubmit:

paster --plugin=ckan datapusher resubmit -c /etc/ckan/ckan.ini
