# propane
Propane is a demo data generator for ALM Octane. It is a single postman collection, leverages a single postman environment and runs via Newman. 


## utilize me

You can [download and install](https://nodejs.org/en/download/current/) Node.js on Linux, Windows, and Mac OSX. After you install Node.js, Newman is just a command away. Install Newman from npm globally on your system, which allows you to run it from anywhere.

```
$ npm install -g newman 
```

Put the files in a tasty directory. Here's the command to run.

```
[demo@nimbusserver ~]$ newman run propane-15-1-66-45-beta.postman_collection.json -e propane.postman_environment.json --delay-request 1000 
```
