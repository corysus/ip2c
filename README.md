# ip2c Node Module

Node.js module for resolve IPs to country codes/names using [ip2c.org](https://ip2c.org) service.

## Install
    npm i ip2c

## Usage
````javascript
    const ip2c = require('ip2c')
    ip2c('ip_address').then(data => {
        console.log(data)
        /* return obj:
            {
                status: 200,
                headers: {...},
                data: { code: 'XX', iso: 'XXX', fullname: 'XXXXX' }
            }
        */
    }).catch(err => console.log('error', err))
````