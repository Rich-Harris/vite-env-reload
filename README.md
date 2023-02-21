# vite-env-reload

Repro for https://github.com/vitejs/vite/issues/12127.

```
git clone git@github.com:Rich-Harris/vite-env-reload
cd vite-env-reload
npm i
npm start
```

While running the dev server, create an `.env` file. Nothing happens.

Edit the `.env` file to include a message like `VITE_MESSAGE=hello`. The server restarts, and the message is printed below.

Edit the message. The server restarts.

Delete the `.env` file. The server does not restart.
