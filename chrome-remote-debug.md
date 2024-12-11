# Start chrome in remote debugging mode
```
start chrome --remote-debugging-port=9222 --remote-debugging-address=0.0.0.0  --remote-allow-origins=* --no-sandbox
```
# Install ngrok
# Config ngrok
```
ngrok http 9222 --host-header="localhost:9222"
```

From your machine
Access to ngrok endpoint https://xxxx.ngrok-free.app/json
Get the value of devtoolsFrontendUrl. It looks like `/devtools/inspector.html?ws=localhost:9222/devtools/page/43DFE7876AD3017E01BA0E3E527A8EFB`
Navigate to 
https://xxxx.ngrok-free.app//devtools/inspector.html?wss=xxxx.ngrok-free.app/devtools/page/43DFE7876AD3017E01BA0E3E527A8EFB
