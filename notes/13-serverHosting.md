cloudflare - website for domain name hosting and ssl





ssl generation - on cloudflare
  ssl/tls
    origin server
      generate private key and csr with cloudflare
      create certificate
        origin certificate and private certificate - need to be put on your box that is being hosted.
          "
          sudo nano etc/nginx/sites-available/default #changing the settings here to be suitable with https settings. adding a reroute form port 80 to port 443
          "
          sudo nano etc/ssl/(certificate name) #adjust the content to fit your origin cert
          sudo nano etc/ssl/(private key name) #adjust the content to fit your private key
          sudo nginx -t #checking to see if syntax is ok and it accepted the certs and keys

          docker is a software designs for creating a pre-setups for instances of applications
          FOR INFORMATION ON DOCKER GO TO: https://www.digitalocean.com/community/tutorials/working-with-docker-containers

          FOR CLOUDFLARE DOMAIN NAME