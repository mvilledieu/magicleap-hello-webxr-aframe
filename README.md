
# Magic Leap Helio - Hello WebXR (aframe.js)

Hello World, made using a custom version of **[aframe.js v0.9.2](https://github.com/mvilledieu/aframe/tree/magicleap-helio-aframe-support)** adding compatibility to  **aframe** to the version of the WebXR API used by Helio (Based on chrome m73).

## Try "Hello WebXR" on device:

To try it out on device open [helio](https://www.magicleap.com/experiences/helio) and go to that link:

https://bit.ly/2WWVHak
or
https://mvilledieu.github.io/magicleap-hello-webxr-aframe/

## Fork (Remix) and live edit this example:

[![Remix on Glitch](https://cdn.glitch.com/2703baf2-b643-4da7-ab91-7ee2a2d00b5b%2Fremix-button.svg)](https://glitch.com/edit/#!/remix/magicleap-hello-webxr-aframe)

 
## Local server:

For local testing/serving you'll need to generate a `cert.pem` and `key.pem` and put them at the root of your folder. The npm module `http-server` needs it to be able to serve your files over https (Required by WebXR).

```sh
$ openssl req -newkey rsa:2048 -new -nodes -x509 -days 3650 -keyout key.pem -out cert.pem
$ yarn
$ yarn serve
```

Once you see the `Your connection is not private` message please click on `advanced` and `Proceed to 127.0.0.1 (unsafe)` and have fun!
