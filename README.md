# Alpaca Trade API Node

Node.js library for Alpaca Trade API.

## API Documentation

The REST API documentation can be found in https://docs.alpaca.markets.

## Installation

```sh
npm install --save alpaca-trade-api
```

## Usage

* Require 'alpaca-trade-api' in your file.

  ```js
  var alpaca = require('alpaca-trade-api');
  ```
* Set API config options (base_url, key_id, secret_key).

  ```js
  alpaca.configure({
    baseUrl: 'https://api.alpaca.markets', /* Optional: defaults to https://api.alpaca.markets */
    keyId: 'AKFZXJH121U18SHHDRFO',
    secretKey: 'pnq4YHlpMF3LhfLyOvmdfLmlz6BnASrTPQIASeiU'
  });
  ```
* Call methods, which will return a promise.

  ```js
  alpaca.getAccount().then((account) => {
    console.log('Current Account:', account);
  })
  ```

## Methods

### Account API
* `getAccount()`: Calls `GET /account` and returns an account.

### Orders API

### Positions API

### Assets API

### Calendar API