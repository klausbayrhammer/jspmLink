# How to reproduce

Executing `jspm link` fails with the following error message as long as the `lib/` directory doesn't exist

```
err  Error: TypeError: msg.replace is not a function
         at moduleMsg (/.npm-global/lib/node_modules/jspm/lib/ui.js:104:6)
         at Object.exports.format.err (/.npm-global/lib/node_modules/jspm/lib/ui.js:67:45)
         at Object.exports.log (/.npm-global/lib/node_modules/jspm/lib/ui.js:92:23)
         at /.npm-global/lib/node_modules/jspm/lib/link.js:113:8
         at lib$rsvp$$internal$$tryCatch (/.npm-global/lib/node_modules/jspm/node_modules/rsvp/dist/rsvp.js:493:16)
         at lib$rsvp$$internal$$invokeCallback (/.npm-global/lib/node_modules/jspm/node_modules/rsvp/dist/rsvp.js:505:17)
         at lib$rsvp$$internal$$publish (/.npm-global/lib/node_modules/jspm/node_modules/rsvp/dist/rsvp.js:476:11)
         at lib$rsvp$$internal$$publishRejection (/.npm-global/lib/node_modules/jspm/node_modules/rsvp/dist/rsvp.js:419:7)
         at lib$rsvp$asap$$flush (/.npm-global/lib/node_modules/jspm/node_modules/rsvp/dist/rsvp.js:1198:9)
         at doNTCallback0 (node.js:408:9)
         at /.npm-global/lib/node_modules/jspm/node_modules/systemjs-builder/lib/builder.js:23:9
         at Object.lib$rsvp$events$$default.trigger (/.npm-global/lib/node_modules/jspm/node_modules/rsvp/dist/rsvp.js:245:13)
         at null._onTimeout (/.npm-global/lib/node_modules/jspm/node_modules/rsvp/dist/rsvp.js:779:47)
```