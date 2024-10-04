const Websocket = require("ws");
var http = require('http');
const wss = new Websocket.Server({port: 8080});



wss.on("connection", function connection(ws) {
    ws.on("message", function incoming(message) {
        console.log("received: %s", message);

        ws.send("Hello from the server!");
    })

    ws.send("Welcome to the websocket server");
});
