# Pixlr Editor Premium Spoof

This repository contains a simple script to spoof premium access on [Pixlr Editor](https://pixlr.com/editor/).

## Requirements

You must be logged into any Pixlr account for the script to work.

## Usage

1. Log in to any Pixlr account.
2. Inject the following code into your browser's developer console:

```javascript
window.webpackChunkpixlr.push([
    [Math.random()],
    {},
    async req => {
        var y = await req(79453);
        y.N.subscription = true;
        y.N.subscriptionAccess = "premium";
    },
]);
```

Once executed, the script will grant your session "premium" subscription access.

> **Note:** This is for educational and testing purposes only. Use responsibly.
