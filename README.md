# DeroGold Blockchain Cache API

## Prerequisites

* MariaDB/MySQL with InnoDB support
* [RabbitMQ](https://www.rabbitmq.com/)
* [DeroGold: Blockchain Data Collection Agent]()
* [DeroGold: Blockchain Relay Agent]()
* [Node.js](https://nodejs.org/) LTS

## Foreword

We know that this documentation needs cleaned up and made easier to read. We'll compile it as part of the full documentation as the project moves forward.

## Setup

1) Clone this repository to wherever you'd like the API to run:

```bash
git clone https://github.com/derogold/blockchain-cache-api.git
```

2) Install the required Node.js modules

```bash
cd blockchain-cache-api && npm install
```

3) Use your favorite text editor to change the values as necessary in `config.json`

**Note:** Make sure you use a read-only database user for security reasons

```javascript
{
  "bindIp": "0.0.0.0",
  "httpPort": 80,
  "corsHeader": "*"
}
```

4) Fire up the script

```bash
export RABBIT_PUBLIC_SERVER=localhost
export RABBIT_PUBLIC_USERNAME=yourrabbitmqusername
export RABBIT_PUBLIC_PASSWORD=yourrabbitmqpassword
export MYSQL_HOST=localhost
export MYSQL_PORT=3306
export MYSQL_USERNAME=yourdbusername
export MYSQL_PASSWORD=yourdbpassword
export MYSQL_DATABASE=yourdbname
node index.js
```

## API

The documentation for the full REST API provided by this package is work in progress. If you'd like to help with the documenting, 
give us a shout on our Discord in dev-talk channel. 

Original version, courtesy of now non-existent:
###### (c) 2018-2019 TurtlePay® Development Team

This version is maintained and used by:
###### (c) 2018 - 2024 DeroGold Developers
