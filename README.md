# cryptpad-mongo-store

Storage API for cryptpad implemented using mongodb.

## Status

`cryptpad-mongo-store` is deprecated, and Cryptpad's storage API is liable to change in the future.

This repository is simply for anyone running their own instance of Cryptpad who would prefer to use mongodb instead of the officially supported storage module(s).

Pull requests are very welcome.

## Why?

mongo is the original storage engine for cryptpad

it has been removed as the official storage engine, but it might still work.

## Install

```
cd /path/to/cryptpad;
npm install cryptpad-mongo-store;
```

## Configure

```
{
    storage: 'cryptpad-mongo-store',

    /*  this url is accessible over the internet.
        it is useful for testing but should not be used in production

        it should really be used to refer to a local installation of mongodb
        to install the mongodb client, run npm install mongodb
    */

    mongoUri: 'mongodb://demo_user:demo_password@ds027769.mongolab.com:27769/demo_database',
    mongoCollectionName: 'cryptpad',
}
```

## License

Available under the AGPLv3.0.
