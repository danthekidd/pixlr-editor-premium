# Pixlr Editor Premium Spoof

This repository contains a simple script to spoof premium access on [Pixlr Editor](https://pixlr.com/editor/).

## Requirements

You must be logged into any Pixlr account for the script to work.

## Methods to Get Premium Access

### Method 1: Using the Script

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

### Method 2: Using the Pixlr Premium URL

1. Go to [Pixlr Editor Premium URL](https://dev.pixlr.com/editor/?premium=true).
2. Sign into your Pixlr account.
3. This will automatically activate the premium features for your session.

> **Note:** This is for educational and testing purposes only. Use responsibly.
