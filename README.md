# Aedes

Barebone MQTT server that can run on any stream server.

## Example

```js
var aedes   = require('./aedes')()
  , server  = require('net').createServer(aedes.handle)
  , port    = 1883

server.listen(port, function() {
  console.log('server listening on port', port)
})
```

## Todo

* [x] QoS 0 support
* [x] Retain messages support
* [x] QoS 1 support
* [ ] QoS 2 support
* [x] clean=false support
* [ ] Keep alive support
* [ ] Disconnect other clients with the same client.id
* [ ] mongo persistence (external module)
* [ ] redis persistence (external module)
* [ ] levelup persistence (external module)

## License

MIT
