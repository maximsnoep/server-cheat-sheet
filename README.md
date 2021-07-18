# server cheat sheet

## nginx

create a site: ```sudo cp \etc\nginx\sites-available\default \etc\nginx\sites-available\xxx.com```

edit a site: ```sudo nano \etc\nginx\sites-available\xxx.com```

enable a site: ```sudo ln -s \etc\nginx\sites-available\xxx.com \etc\nginx\sites-enabled\xxx.com```

reload nginx: ```sudo systemctl reload nginx```

## certbot

view all certificates: ```sudo certbot certificates```

create a certificate: ```sudo certbot```

renew a certificate: ```sudo certbot renew```

## pm2

view all processes: ```pm2 list```

create a process: ```PORT=9999 pm2 start index.js --watch --name "XXX.COM"```

