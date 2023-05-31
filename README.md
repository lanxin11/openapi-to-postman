
# Overview

This repository helps you to convert an OpenAPI 3.0 spec, such as the Quickstart API spec ([swaggerv2API.yaml](https://www.zuora.com/developer/yaml/swaggerv2API.yaml)), to a file format that is much easier to be imported into Postman. Also, the code samples are also imported with less manual tweaking work.



## Intallation

To use the converter as a Node module, you need to have a copy of the NodeJS runtime. The easiest way to do this is through npm. If you have NodeJS installed you have npm installed as well.

```terminal
$ npm install openapi-to-postmanv2
```

If you want to use the converter in the CLI, install it globally with NPM:

```terminal
$ npm i -g openapi-to-postmanv2
```


## Usage 

1. Download the OpenAPI spec for the Quickstart API to your local environment. 

2. Change directory to the folder where you store the API spec for the Quickstart API. 

3. In terminal, run the following command:

```terminal
openapi2postmanv2 -s swaggerv2API.yaml -o specv2API.json -p -O folderStrategy=Tags,requestParametersResolution=Example,optimizeConversion=false,stackLimit=100
```

4. To import the collection in Postman, click **Import** in your workspace, then choose the JSON file that the converter generated (specv2API.json). It will take no more than one minute to finish importing.

For more information about commands and other advanced options, check [this repository](https://github.com/postmanlabs/openapi-to-postman).



