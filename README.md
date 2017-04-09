# &#60;dsc-polymer-form-login&#62;

![Build Status](https://travis-ci.org/discovery-tecnologia/dsc-polymer-form-login.svg?branch=master)
![Bower version](https://img.shields.io/bower/v/dsc-polymer-form-login.svg)
[![npm](https://img.shields.io/npm/l/express.svg)]()

Basic and standard form login component with Polymer. This project use Google Material Design.

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
<dsc-polymer-form-login language="br" 
                        method="POST"
                        endpoint="http://my-site/my-api" 
                        headers='{"X-foo": "X-bar"}'
                        on-request-sending="myHandlerRequestFunction"
                        on-response-success="myHandlerReponseFunction"></dsc-polymer-form-login>
```

## API

### Property
| Name     | Type    | Description                           | Default                           |
|:---------|---------|---------------------------------------|-----------------------------------|
| language | String  |Translate the form messages and labels | en                                |
| endpoint | String  |Endpoint API                           | http://localhost:3000/api/login   |
| method   | String  |String method used                     | POST                              |
| headers  | Object  |Headers options for requisition        | null                              |

### Events
| Name             | Description                                                                      |
|:-----------------|----------------------------------------------------------------------------------|
| request-sending  | Listen to the request event. Provides the request object to another element.     |
| response-success | Listen to the response event ok. Provides the response object to another element.|

The file [locales.json](https://github.com/discovery-tecnologia/dsc-polymer-form-login/blob/master/locales.json) contains the map of languages translated (EN,BR,ES).

## Test

Check sintax and execute selenium tests.

```
$ npm test
```

## TODO

 * more tests
