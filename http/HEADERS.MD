# Headers


### Can't see some headers

if you cant see some headers on client side,  set that header name with Access-Control-Expose-Headers.

  ```
  Access-Control-Expose-Headers=Authorization: X-Custom-header
  ```
In PHP
```php
header("Access-Control-Expose-Headers: Authorization, X-Custom-header")
```
