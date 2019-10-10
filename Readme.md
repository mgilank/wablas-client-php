# (Unofficial) Wablas PHP Client - Fork dari Saputradharma

Edited (10/10/2019)
- new url (console.wablas.com)
- some minor change 

## Install
```php
composer require wablas/wablas-client-php
```

## Usage 
Please register at [Wablas](https://wablas.com/) to get your `apiToken`.
```php
use Wablas\WablasClient;

$apiToken = 'your-api-token-here';
$wablasClient = new WablasClient($apiToken);

// add recipient (support multiple recipient)
$wablasClient->addRecipient('08xxxxxxxxx');

// send message
$message = 'type your message here.';
$wablasClient->sendMessage($message);

// send image
$wablasClient->sendImage('your image caption here', 'http://your.image/url/here')
```

