![LUSID_by_Finbourne](https://content.finbourne.com/LUSID_repo.png)

[![Build Status](https://travis-ci.org/finbourne/lusid-sdk-js.svg?branch=master)](https://travis-ci.org/finbourne/lusid-sdk-js)

# LUSID<sup>®</sup> JavaScript SDK

A generated version of the SDK is included in the `sdk` folder based on the OpenAPI specification named `lusid.json` in the root folder.  The most up to date version of the OpenAPI specification can be downloaded from https://api.lusid.com/swagger/v0/swagger.json

The SDK can also be installed using `npm`:

```
$ npm install @finbourne/lusid-preview
```

# Generating the SDK
If you would prefer to generate the Javsscript SDK locally from the FINBOURNE OpenAPI specification, follow these steps:

- download the latest swagger.json file from https://api.lusid.com/swagger/index.html
- save it in this directory as lusid.json
- run `$ docker-compose up && docker-compose rm -f`

# Working with the SDK

The relevant tests are in sdk/test/tutorials

You need to either create a sdk/secrets.json file, or set environment variables, based on your lusid installation. The configurations go into sdk/test/tutorials/clientBuilder.ts

To generate the JS based on TS

```
$ cd sdk/
$ npm i
$ npm run-script build
```

To run all scripts in sdk/test/tutorials

```
$ npm test
```