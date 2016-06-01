Vueify issue
------------

```
$ node -v
v4.4.5
$ npm -v
3.9.3

$ npm install

$ ./node_modules/.bin/browserify -t vueify main.js
Error: Cannot find module 'vueify/node_modules/vue-hot-reload-api' from '/home/djonas/projects/vueify-test'
    at /home/djonas/projects/vueify-test/node_modules/resolve/lib/async.js:46:17
    at process (/home/djonas/projects/vueify-test/node_modules/resolve/lib/async.js:173:43)
    at ondir (/home/djonas/projects/vueify-test/node_modules/resolve/lib/async.js:188:17)
    at load (/home/djonas/projects/vueify-test/node_modules/resolve/lib/async.js:69:43)
    at onex (/home/djonas/projects/vueify-test/node_modules/resolve/lib/async.js:92:31)
    at /home/djonas/projects/vueify-test/node_modules/resolve/lib/async.js:22:47
    at FSReqWrap.oncomplete (fs.js:82:15)

$ grep -F vue-hot-reload-api npm-shrinkwrap.json
    "vue-hot-reload-api": {
      "from": "vue-hot-reload-api@>=1.3.2 <2.0.0",
      "resolved": "http://npm.mirror.lax/vue-hot-reload-api/-/vue-hot-reload-api-1.3.2.tgz"
```
