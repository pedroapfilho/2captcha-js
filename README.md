<h1 align="center">Welcome to 2captcha-node 👋</h1>

<p align="center">
  <a href="https://www.npmjs.com/package/2captcha-node"><img alt="NPM version" src="https://badge.fury.io/js/2captcha-node.svg"></a>
  <a href="https://travis-ci.com/pedroapfilho/2captcha-node"><img alt="TRAVIS version" src="https://travis-ci.com/pedroapfilho/2captcha-node.svg?branch=master"></a>
</p>

> A NodeJS wrapper to solve image captchas with 2captcha

### 🏠 [Homepage](https://github.com/pedroapfilho/2captcha-node#readme)

## Prerequisites:

You will need a `2Captcha API key`

## Install

```sh
npm install
```

## Usage

Set up your api key:

```js
import captchaSolver from "2captcha-node";

const captcha = captchaSolver("your-api-key");
```

It'll return an object with the `solve` function, and you'll be able to use it inside of your script

```js
const options = {
  image: "base64-image",
  maxAttempts: 60 // Optional
};

const solvedCaptcha = await captcha.solve(options);
```

And this solvedCaptcha will be the string of your resolved captcha

You can use the `balance` function too, to see your balance at 2Captcha

```js
const balance = await captcha.balance();
```

## Author

👤 **Pedro Filho <pedro@filho.me>**

- Twitter: [@pedrofilhome](https://twitter.com/pedrofilhome)
- Github: [@pedroapfilho](https://github.com/pedroapfilho)

## 🤝 Contributing

Contributions, issues and feature requests are welcome!<br />Feel free to check [issues page](https://github.com/pedroapfilho/2captcha-node/issues).

## Show your support

Give a ⭐️ if this project helped you!

<a href="https://www.buymeacoffee.com/khcUAVF" target="_blank"><img src="https://bmc-cdn.nyc3.digitaloceanspaces.com/BMC-button-images/custom_images/orange_img.png" alt="Buy Me A Coffee" style="height: auto !important;width: auto !important;" ></a>
