```mermaid
sequenceDiagram
    participant Attacker
    participant WebConsumer
    participant BotNet
    participant Firewall
    participant WebServer
    Attacker->>BotNet:Engage Attack on WebServer
    BotNet->>Firewall:Create and send mass connections to Webserver
    WebConsumer->>Firewall:Attempt Connection to Webserver
    Firewall->>WebServer:If WebConsumer allow connection
    Firewall->>BotNet:If BotNet Detected reject Connection
```

##DDOS Sequence
An attacker will utilize a Bot Net already created to disrupt service on a particular website</br>

* That attacker will tell the botnet to send multiple connection requests to a specific website or service
* The BotNet will attempt to connect multiple times at the same instant to overwhelm the site or service
* The Firewall will filter all the data incoming to the site or server for malicious intent and reject those it deems bad

