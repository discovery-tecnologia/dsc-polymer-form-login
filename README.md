# &#60;dsc-polymer-form-login&#62;

![Build Status](https://travis-ci.org/discovery-tecnologia/dsc-polymer-form-login.svg?branch=master)
![Bower version](https://img.shields.io/bower/v/dsc-polymer-form-login.svg)
[![npm](https://img.shields.io/npm/l/express.svg)]()

Basic and standard form component with Polymer. This project use Google Material Design.

![demo](https://raw.githubusercontent.com/discovery-tecnologia/dsc-polymer-form-login/master/docs/img/form.png)

## Demo

```
$ git clone https://github.com/discovery-tecnologia/dsc-polymer-form-login.git
$ cd dsc-polymer-form-login
$ npm install
$ npm install -g polymer-cli
$ polymer serve
```
Open browser: http://localhost:8080/components/dsc-polymer-form-login/demo/index.html

## Usage

Install with:

```
$ bower i dsc-polymer-form-login --save
```

Example usage:

```html
<dsc-polymer-form-login language="br" endpoint="http://my-site/my-api"></dsc-polymer-form-login>
```

## API

| Property       | Description                            | Default                           |
|:---------------|----------------------------------------|-----------------------------------|
| language       | Translate the form messages and labels | en                                |
| endpoint       | Endpoint API                           | http://localhost:3000/api/contact |

The file [locales.json](https://github.com/discovery-tecnologia/dsc-polymer-form-login/blob/master/locales.json) contains the map of languages translated (EN,BR,ES).

## Test

Check sintax and execute selenium tests.

```
$ npm test
```

## TODO

 * more tests
