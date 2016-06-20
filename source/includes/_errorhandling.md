# Error messages and registries in the iLO RESTful API
> HTTP response 400

```json
{
  "error": {
    "@Message.ExtendedInfo": [
      {
        "MessageId": "iLO.0.9.InvalidLicenseKey"
      }
    ],
    "code": "iLO.0.10.ExtendedInfo",
    "message": "See @Message.ExtendedInfo for more information."
  }
}
```

```
"InvalidLicenseKey": {
    "Description": "The license key is not valid.",
    "Message": "The license key is not valid.",
    "Severity": "Warning",
    "NumberOfArgs": 0,
    "ParamTypes": [],
    "Resolution": "Retry the operation using a valid license key."
}
```

Error messages appear in several places in the iLO RESTful API.

* An immediate response to an HTTP operation.
* A `SettingsResult` in the data model where other providers, such as BIOS, processed the settings at some point and want to communicate status in the model.

All error cases use a basic error JSON structure called `ExtendedInfo`.  The most important property in `ExtendedInfo` is `MessageId`, a string containing a lookup key into a message registry.

`MessageId` helps to keep the iLO service small by keeping much of the explanatory text for an error out of the code. Instead, iLO supplies an `ExtendedInfo` response, where the `MessageId` provides enough information so that you can look up more details from another file.

For example, if you `POST` to the iLO license service to install an iLO license, but you supply an incorrect `LicenceKey` string, iLO responds with an error similar to the following:

HTTP response 400 is the standard RESTful API response to an error. In the example above, the error is easy to understand, but some errors are not easy to understand. To display a more meaningful error message, parse the string `iLO.0.9.InvalidLicenseKey` into the following
components:

* `iLO.0.9`—This is the base name of the message registry to consult. Look for a matching registry file.
* `InvalidLicenseKey`—This is the lookup key into the message registry.

The search returns a result similar to the following:

Many error messages can also return parameters. These parameters may be plugged into the
strings in the registry to form detailed messages tailored to the instance of the error message.







