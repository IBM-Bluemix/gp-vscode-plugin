# Globalization Pipeline Extension README

This extension enables you to quickly create, upload, and delete translation bundles in the Globalization Pipeline service on IBM Bluemix.

## Features

You can create a new bundle right from the editor without having to use the Globalization Pipeline service's dashboard

![create bundle](images/create_bundle.png)

You can upload your content from the editor as well and the extension will automatically get all your available bundles.

![upload bundle](images/upload_bundle.png) 

## Requirements

You must first create an instance of the Globalization Pipeline service on Bluemix before you can use this extension to work with translation bundles.

## Extension Settings

To use the extension copy over your VCAP credential settings for the Globalization Pipeline service and fill in the appropriate fields.

This extension contributes the following settings:

* `g11n.userId`: The Globalization Pipeleine service userId
* `g11n.password`: The Globalization Piepeline service password
* `g11n.instanceId`: The Globalization Pipeline service instanceId
* `g11n.url`: The Globalization Pipeline service url end point
* `g11n.sourceLanguage`: The source language of the content that you will upload to the service, e.g. *en*, must be a valid BCP 47 language code. By default this value is to *en*
* `g11n.targetLanguages`: An array of target lanaguges that your bundle will be translated into, e.g., *['es', 'fr']*, must be valid BCP 47 lanaguge codes

## Usage

In the command palette `(F1)` type Globalization Pipeline you should see the following commands:

+ Globalization Pipeline - Create Bundle
- Globalization Pipeline - Upload Source Bundle
* Globalization Pipeline - Delete Bundle

When you use these commands a connection will automatically be made to the Globalization Pipeline service on IBM Bluemix to complete your requested action.
When you upload your source bundle content the extension will automatically detect the file format and will perform any necessary transformation for you. 
Currently only Java properties, JSON, and i18n AMD resource bundles are supported.


## Release Notes

No additional release notes at this time.

### 0.0.1

Initial release of Globalization Pipeleine extension
