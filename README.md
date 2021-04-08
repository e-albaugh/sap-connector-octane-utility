# propane
*propane* is a demo data generator for ALM Octane. It is a single postman collection, leveraging a single postman environment, run via Newman. It is purpose built for [admpresales](https://hub.docker.com/u/admpresales), but can be extended to run against any Octane environment this side of the Mississippi.

## install newman
You can [download and install](https://nodejs.org/en/download/current/) Node.js on Linux, Windows, and Mac OSX. After you install Node.js, Newman is just a command away. Install Newman from npm globally on your system, which allows you to run it from anywhere.

```
$ npm install -g newman 
```

## use me
Put the files in a tasty directory. Run it like a gas grill.

```
$ newman run propane.postman_collection.json -e propane.postman_environment.json --delay-request 1000 

...
...
...

===================================================================
                              executed |                   failed |
-------------------------------------------------------------------
          iterations |               1 |                        0 |
-------------------------------------------------------------------
            requests |             259 |                        0 |
-------------------------------------------------------------------
        test-scripts |             238 |                        0 |
-------------------------------------------------------------------
  prerequest-scripts |             176 |                        0 |
-------------------------------------------------------------------
          assertions |               0 |                        0 |
-------------------------------------------------------------------
total run duration: 5m 43s                                        |
-------------------------------------------------------------------
total data received: 6.4MB (approx)                               | 
-------------------------------------------------------------------
average response time: 657ms [min:32ms, max: 1m 1.9s, s.d.: 4.4s] |
===================================================================
```
