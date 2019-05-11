1. Put the password for the mysql user in db.env
2. Put the password for the mysql root user in docker-compose.yml
3. Edit the domain name in docker-compose.yml (service app labels)
4. docker-compose pull
5. docker-compose build
6. docker-compose up -d
7. Complete nexcloud web setup
8. Add/edit the following two lines in ./data/nextcloud/config/config.php with the IP of your server and domain name
   'trusted_proxies' => ['1.1.1.1'],
   'overwriteprotocol' => 'https',
   'overwrite.cli.url' => 'https://example.com',
9. docker-compose restart
10. Profit
