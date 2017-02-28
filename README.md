# Gulpfile.js
Gulpfile.js template

```bash
curl -sSL https://rawgit.com/start-project/Gulpfile.js/init | sh [-s -- -h]
```

### Config file:
##### Gulpfile.json
```json
{
    "path": {
        "src": "./src",
        "root": "./",
        "dist": "./assets/"
    },
    "proxy": {
        "protocol": "http://",
        "path": "localhost",
        "port": 8888
    },
    "gitignore": true
}
```
* path {Object} - paths list
    * path.src {String} - sources
    * path.root {String} - project root
    * path.dist {String} - destination directory
* proxy {Object | False} - proxy params
    * proxy.protocol {String} - local protocol
    * proxy.path {String} - local url
    * proxy.port {Integer} - local port
* gitignore {Boolean} - adding dist to .gitignore

### Gulp tasks
* default ["build", "watch"]
* build ["stylus", "js", "other"]
