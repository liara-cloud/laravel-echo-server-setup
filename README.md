# Deploy Laravel Echo Server to Liara

1) Create a new project in Liara's console.

2) Clone this repository and `cd` into it.

3) Install dependencies using `npm install` command.

4) Create a new client ID using: `npx laravel-echo-server client:add APP_ID`

If you run client:add without an app id argument, one will be generated for you. After running this command, the client id and key will be displayed and stored in the laravel-echo-server.json file.

5) Open project's settings in Liara's console and add the following environment variables:

```
LARAVEL_ECHO_SERVER_AUTH_HOST=https://my-laravel-app.liara.run
LARAVEL_ECHO_SERVER_REDIS_HOST=s8.liara.ir
LARAVEL_ECHO_SERVER_REDIS_PORT=5566
LARAVEL_ECHO_SERVER_REDIS_PASSWORD=secret
```

6) Deploy the echo server using `liara deploy`.
