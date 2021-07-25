# sap-connector-octane-utility
The *sap-connector-octane-utility* generates the necessary fields and forms in ALM Octane utilized by the sap connector. It is a single postman collection, leveraging a single postman environment, run via Newman. It is purpose built for [diff consulting](https://www.diffc.com/) dev environments, but can be extended to run against any Octane environment. 

## install newman
You can [download and install](https://nodejs.org/en/download/current/) Node.js on Linux, Windows, and Mac OSX. After you install Node.js, Newman is just a command away. Install Newman from npm globally on your system, which allows you to run it from anywhere.

```
$ npm install -g newman 
```

## customize to your environment
Ensure the values (baseUrl, port, ssid, wsid, etc.) in the [sap-connector-octane-utility](https://github.com/e-albaugh/sap-connector-octane-utility/blob/main/sap-connector-octane-utility.postman_environment.json) are filled out according to your environment. The utility will not work if you do not do this. 

## use me
Put the files in a tasty directory. Run it like a gas grill.

```
$ newman run sap-connector-octane-utility.postman_collection.json -e sap-connector-octane-utility.postman_environment.json --delay-request 500

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
