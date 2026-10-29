Backend: It's a computer listening to HTTP/Websocket or any other request through a port. It provides with files and with these ports it connects to other computers through the internet.

DNS (Domain Name Server): Have different types of records.
* Have an open port at 443 and 80 so requests can reach our server.

As for the request:
* It starts on the browser.
* It goes to the DNS server.
* Then goes to the AWS server.
* Goes through a firewall.
* Reaches our AWS instance.
* The request reaches nginx.
* It finally forwards to our localhost:3001, our final server.

Why can't we write backend logic in front-end?
1) Security reasons: A browser is restrictive in the way of accessing things like files to write logs.
2) CORS (Cross-Origin Resource Sharing)
3) Databases: Drivers that let you connect to databases in an efficient way.
4) Computing power.