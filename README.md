# propane
Propane is a demo data generator for ALM Octane. It is a single postman collection, leverages a single postman environment and runs via Newman. It is purpose built for nimbus, but can be extended to run against any Octane environment this side of the Mississippi.

## install newman
You can [download and install](https://nodejs.org/en/download/current/) Node.js on Linux, Windows, and Mac OSX. After you install Node.js, Newman is just a command away. Install Newman from npm globally on your system, which allows you to run it from anywhere.

```
$ npm install -g newman 
```

## use me
Put the files in a tasty directory. Run it like a gas grill.

```
$ newman run propane-15-1-66-45-beta.postman_collection.json -e propane.postman_environment.json --delay-request 1000 
```
