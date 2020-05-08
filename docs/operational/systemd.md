# Creating a systemd file
[Tutorial](https://www.shellhacks.com/systemd-service-file-example/)

[Service file template (Kudos Ward)](https://gist.github.com/WardToulet/93cbe888dc18e9cc531c31636591d40c)


## Mogelijke error

Als je een error krijgt kan het zijn dat je docker-compose installatie op een andere plaats staat
controleer effe of die in

`/usr/local/bin/docker-compose`

of in

`/usr/bin/docker-compose`

en pas dit dan ook aan in de .service file