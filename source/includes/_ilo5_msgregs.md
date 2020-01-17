
### Base.1.4.AccessDenied
While attempting to access, connect to, or transfer to/from another resource, the service was denied access.

| | |
|:---|:---|
|Message Format|"While attempting to establish a connection to %1, the service was denied access."
|Severity|Critical
|Resolution|Verify that the URI is correct and that the service has the appropriate credentials.

### Base.1.4.AccountForSessionNoLongerExists
The account for the current session is removed, and the current session is also removed.

| | |
|:---|:---|
|Message Format|"The account for the current session is removed, and the current session is also removed."
|Severity|OK
|Resolution|Attempt to connect using a valid account.

### Base.1.4.AccountModified
The account was modified successfully.

| | |
|:---|:---|
|Message Format|"The account was modified successfully."
|Severity|OK
|Resolution|None.

### Base.1.4.AccountNotModified
The request was unable to modify the account.

| | |
|:---|:---|
|Message Format|"The account modification request did not complete."
|Severity|Warning
|Resolution|If the operation did not complete, check the authorization or the request body for issues and resubmit the request.

### Base.1.4.AccountRemoved
The account was removed successfully.

| | |
|:---|:---|
|Message Format|"The account was removed successfully."
|Severity|OK
|Resolution|None.

### Base.1.4.ActionNotSupported
The action supplied in the POST operation is not supported by the resource.

| | |
|:---|:---|
|Message Format|"The action %1 is not supported by the resource."
|Severity|Critical
|Resolution|The action was invalid or the wrong resource was the target. See the implementation documentation for assistance.

### Base.1.4.ActionParameterDuplicate
The action was submitted with a duplicate parameter in the request body.

| | |
|:---|:---|
|Message Format|"The action %1 was submitted with more than one value for the parameter %2."
|Severity|Warning
|Resolution|Resubmit the action with only one instance of the parameter in the request body.

### Base.1.4.ActionParameterMissing
The requested action is missing a parameter that is required to process the action.

| | |
|:---|:---|
|Message Format|"The action %1 requires that the parameter %2 be present in the request body."
|Severity|Critical
|Resolution|Resubmit the action with the required parameter in the request body.

### Base.1.4.ActionParameterNotSupported
The action parameter is not supported on the target resource.

| | |
|:---|:---|
|Message Format|"The parameter %1 for the action %2 is not supported on the target resource."
|Severity|Warning
|Resolution|If the operation did not complete, remove the parameter and resubmit the request.

### Base.1.4.ActionParameterUnknown
An action was submitted, but a supplied parameter did not match any of the known parameters.

| | |
|:---|:---|
|Message Format|"The action %1 was submitted with the invalid parameter %2."
|Severity|Warning
|Resolution|If the operation did not complete, correct the invalid parameter and resubmit the request.

### Base.1.4.ActionParameterValueFormatError
The value type is correct, but the format is not supported or the size/length is exceeded.

| | |
|:---|:---|
|Message Format|"The value %1 for the parameter %2 in the action %3 is in a format that is not supported by the parameter."
|Severity|Warning
|Resolution|If the operation did not complete, correct the parameter value in the request body and resubmit the request.

### Base.1.4.ActionParameterValueTypeError
The parameter contains an incorrect value type. For example, a number value for a string parameter type.

| | |
|:---|:---|
|Message Format|"The value %1 for the parameter %2 in the action %3 is the incorrect parameter type."
|Severity|Warning
|Resolution|If the operation did not complete, correct the parameter value in the request body and resubmit the request.

### Base.1.4.CouldNotEstablishConnection
An attempt to access the resource, image, or file at the URI was unsuccessful because a session could not be established.

| | |
|:---|:---|
|Message Format|"The service was unable to establish a connection with the URI %1."
|Severity|Critical
|Resolution|Verify that the URI contains a valid and reachable node name, protocol information, and other URI components.

### Base.1.4.CreateFailedMissingReqProperties
A create operation was attempted on a resource, but a required property was missing from the request.

| | |
|:---|:---|
|Message Format|"The create operation did not complete because the required property %1 was missing from the request."
|Severity|Critical
|Resolution|If the operation did not complete, include the required property with a valid value in the request body and resubmit the request.

### Base.1.4.CreateLimitReachedForResource
Additional resources cannot be created.

| | |
|:---|:---|
|Message Format|"Additional resources cannot be created."
|Severity|Critical
|Resolution|If the operation did not complete, delete resources and resubmit the request.

### Base.1.4.Created
The resource has been created successfully.

| | |
|:---|:---|
|Message Format|"The resource has been created successfully."
|Severity|OK
|Resolution|None

### Base.1.4.EmptyJSON
Indicates that the request body contained an empty JSON object when one or more properties are expected in the body.

| | |
|:---|:---|
|Message Format|"The request body submitted contained an empty JSON object and the service is unable to process it."
|Severity|Warning
|Resolution|Add properties in the JSON object and resubmit the request.

### Base.1.4.EventSubscriptionLimitExceeded
The event subscription establishment has been requested, but the operation did not complete. The number of simultaneous subscriptions exceeded the maximum number allowed by the implementation.

| | |
|:---|:---|
|Message Format|"The event subscription did not complete because the number of simultaneous subscriptions exceeded the maximum number allowed by the implementation."
|Severity|Critical
|Resolution|Before attempting to establish the event subscription, reduce the number of subscriptions or increase the maximum number of simultaneous subscriptions allowed (if supported).

### Base.1.4.GeneralError
Indicates that a general error has occurred.  Use in ExtendedInfo is discouraged.  When used in ExtendedInfo, implementations are expected to include a Resolution property with this error to indicate how to resolve the problem.

| | |
|:---|:---|
|Message Format|"A general error has occurred. See Resolution for information on how to resolve the error."
|Severity|Critical
|Resolution|None.

### Base.1.4.InsufficientPrivilege
The account or credentials associated with the current session are not authorized to perform the requested operation.

| | |
|:---|:---|
|Message Format|"The account or credentials associated with the current session are not authorized to perform the requested operation."
|Severity|Critical
|Resolution|Retry the operation with an authorized account or credentials.

### Base.1.4.InternalError
The request did not complete due to an unknown internal error, but the service is still operational.

| | |
|:---|:---|
|Message Format|"The request failed due to an internal service error, but the service is still operational."
|Severity|Critical
|Resolution|Resubmit the request. If the problem persists, consider resetting the service.

### Base.1.4.InvalidIndex
The Index is not valid.

| | |
|:---|:---|
|Message Format|"The Index %1 is not a valid offset into the array."
|Severity|Warning
|Resolution|Verify the index value provided is within the bounds of the array.

### Base.1.4.InvalidObject
The object is not valid.

| | |
|:---|:---|
|Message Format|"The object at %1 is not valid."
|Severity|Critical
|Resolution|If the operation did not complete, the object is malformed or the URI is incorrect. Make the appropriate corrections and resubmit the request.

### Base.1.4.MalformedJSON
The request body contains malformed JSON.

| | |
|:---|:---|
|Message Format|"The request body submitted is malformed JSON and cannot be parsed by the receiving service."
|Severity|Critical
|Resolution|Verify that the request body is valid JSON and resubmit the request.

### Base.1.4.NoOperation
Indicates that the requested operation will not perform any changes on the service.

| | |
|:---|:---|
|Message Format|"The request body submitted contain no data to act upon and no changes to the resource took place."
|Severity|Warning
|Resolution|Add properties in the JSON object and resubmit the request.

### Base.1.4.NoValidSession
The operation did not complete because a valid session is required in order to access resources.

| | |
|:---|:---|
|Message Format|"There is no valid session established with the implementation."
|Severity|Critical
|Resolution|Establish a session before attempting any operations.

### Base.1.4.PropertyDuplicate
A duplicate property is in the request body.

| | |
|:---|:---|
|Message Format|"The property %1 is duplicated in the request."
|Severity|Warning
|Resolution|If the operation did not complete, remove the duplicate property from the request body and resubmit the request.

### Base.1.4.PropertyMissing
The request does not include a required property.

| | |
|:---|:---|
|Message Format|"The property %1 is a required property and must be included in the request."
|Severity|Warning
|Resolution|If the operation did not complete, verify the property is in the request body and has a valid value.

### Base.1.4.PropertyNotWritable
The request included a value for a read-only property.

| | |
|:---|:---|
|Message Format|"The property %1 is a read-only property and cannot be assigned a value."
|Severity|Warning
|Resolution|If the operation did not complete, remove the property from the request body and resubmit the request.

### Base.1.4.PropertyUnknown
An unknown property is in the request body.

| | |
|:---|:---|
|Message Format|"The property %1 is not valid for this resource."
|Severity|Warning
|Resolution|If the operation did not complete, remove the unknown property from the request body and resubmit the request.

### Base.1.4.PropertyValueFormatError
The value type is correct, but the format is not supported or the size/length is exceeded.

| | |
|:---|:---|
|Message Format|"The value %1 for the property %2 is in a format that is not supported by the property."
|Severity|Warning
|Resolution|If the operation did not complete, correct the property value in the request body and resubmit the request.

### Base.1.4.PropertyValueModified
Indicates that a property was given the correct value type but the value of that property was modified.  Examples are truncated or rounded values.

| | |
|:---|:---|
|Message Format|"The property %1 was assigned the value %2 due to modification by the service."
|Severity|Warning
|Resolution|No resolution is required.

### Base.1.4.PropertyValueNotInList
The value type is correct, but the value is not supported.

| | |
|:---|:---|
|Message Format|"The value %1 for the property %2 is not valid."
|Severity|Warning
|Resolution|If the operation did not complete, choose a value from the enumeration list and resubmit your request.

### Base.1.4.PropertyValueTypeError
The property value contains an incorrect property type. For example, a number value for a string property type.

| | |
|:---|:---|
|Message Format|"The value %1 for the property %2 is the incorrect property type."
|Severity|Warning
|Resolution|If the operation did not complete, correct the property value in the request body and resubmit the request.

### Base.1.4.QueryNotSupported
The query is not supported by the implementation.

| | |
|:---|:---|
|Message Format|"Querying is not supported by the implementation."
|Severity|Warning
|Resolution|If the operation did not complete, remove the query parameter and resubmit the request.

### Base.1.4.QueryNotSupportedOnResource
The query is not supported on the resource. For example, a start/count query is attempted on a resource that is not a collection.

| | |
|:---|:---|
|Message Format|"Querying is not supported on the requested resource."
|Severity|Warning
|Resolution|If the operation did not complete, remove the query parameters and resubmit the request.

### Base.1.4.QueryParameterOutOfRange
The query parameter value is out of range for the resource. For example, a page is requested that is outside the valid page range.

| | |
|:---|:---|
|Message Format|"The value %1 for the query parameter %2 is out of range %3."
|Severity|Warning
|Resolution|Specify a query parameter value that is within range. For example, a page that is within the valid range of pages.

### Base.1.4.QueryParameterValueFormatError
The value type is correct, but the format is not supported or the size/length was exceeded.

| | |
|:---|:---|
|Message Format|"The value %1 for the parameter %2 is in a format that is not supported by the parameter."
|Severity|Warning
|Resolution|If the operation did not complete, correct the value for the query parameter in the request body and resubmit the request.

### Base.1.4.QueryParameterValueTypeError
The query parameter contains an incorrect value type. For example, a number supplied for a query parameter that requires a string.

| | |
|:---|:---|
|Message Format|"The value %1 for the query parameter %2 is the incorrect type of value for the query parameter."
|Severity|Warning
|Resolution|If the operation did not complete, correct the value for the query parameter in the request body and resubmit the request.

### Base.1.4.ResourceAlreadyExists
Indicates that a resource change or creation was attempted but that the operation cannot proceed because the resource already exists.

| | |
|:---|:---|
|Message Format|"The requested resource of type %1 with the property %2 with the value %3 already exists."
|Severity|Critical
|Resolution|Do not repeat the create operation as the resource has already been created.

### Base.1.4.ResourceAtUriInUnknownFormat
The URI is valid, but the resource or image at that URI is in a format that is not supported by the service.

| | |
|:---|:---|
|Message Format|"The resource at %1 is in a format that is not supported by the service."
|Severity|Critical
|Resolution|Place a resource, image, or file that is supported by the service at the URI.

### Base.1.4.ResourceAtUriUnauthorized
An attempt to access the resource, image, or file at the URI is unauthorized.

| | |
|:---|:---|
|Message Format|"While accessing the resource at %1, the service received an authorization error %2."
|Severity|Critical
|Resolution|Verify that the appropriate access is provided for the service to access the URI.

### Base.1.4.ResourceCannotBeDeleted
A delete operation was attempted on a resource that cannot be deleted.

| | |
|:---|:---|
|Message Format|"The delete request did not complete because the resource cannot be deleted."
|Severity|Critical
|Resolution|Do not attempt to delete a resource that does not support the REST API DELETE operation.

### Base.1.4.ResourceExhaustion
Indicates that a resource could not satisfy the request due to some unavailability of resources.  An example is that available capacity has been allocated.

| | |
|:---|:---|
|Message Format|"The resource %1 was unable to satisfy the request due to unavailability of resources."
|Severity|Critical
|Resolution|Ensure that the resources are available and resubmit the request.

### Base.1.4.ResourceInStandby
Indicates that the request could not be performed because the resource is in standby.

| | |
|:---|:---|
|Message Format|"The request could not be performed because the resource is in standby."
|Severity|Critical
|Resolution|Ensure that the resource is in the correct power state and resubmit the request.

### Base.1.4.ResourceInUse
The request to change the resource was rejected because the resource was in use or in transition.

| | |
|:---|:---|
|Message Format|"The change to the resource did not complete because the resource is in use or in transition."
|Severity|Warning
|Resolution|If the operation did not complete, wait until the resource is free and resubmit the request.

### Base.1.4.ResourceMissingAtURI
The operation expected an image or resource at the provided URI, but found none.

| | |
|:---|:---|
|Message Format|"The resource at the URI %1 was not found."
|Severity|Critical
|Resolution|Place a valid resource at the URI or correct the URI and resubmit the request.

### Base.1.4.ResourceNotFound
Indicates that the operation expected a resource identifier that corresponds to an existing resource but one was not found.

| | |
|:---|:---|
|Message Format|"The requested resource of type %1 named %2 was not found."
|Severity|Critical
|Resolution|Provide a valid resource identifier and resubmit the request.

### Base.1.4.ResourceTypeIncompatible
Indicates that the resource type of the operation does not match that for the operation destination.  Examples of when this can happen include during a POST to a collection using the wrong resource type, an update where the @odata.types do not match or on a major version incompatability.

| | |
|:---|:---|
|Message Format|"The @odata.type of the request body %1 is incompatible with the @odata.type of the resource which is %2."
|Severity|Critical
|Resolution|Resubmit the request with a payload compatible with the resource's schema.

### Base.1.4.ServiceInUnknownState
The operation did not complete because the service is in an unknown state and cannot take incoming requests.

| | |
|:---|:---|
|Message Format|"The operation did not complete because the service is in an unknown state and cannot take incoming requests."
|Severity|Critical
|Resolution|If the operation did not complete, restart the service and resubmit the request.

### Base.1.4.ServiceShuttingDown
The operation did not complete because the service is shutting down.

| | |
|:---|:---|
|Message Format|"The operation did not complete because the service is shutting down and cannot take incoming requests."
|Severity|Critical
|Resolution|If the operation did not complete, resubmit the request when the service is available.

### Base.1.4.ServiceTemporarilyUnavailable
The service is temporarily unavailable.

| | |
|:---|:---|
|Message Format|"The service is temporarily unavailable.  Retry in %1 seconds."
|Severity|Critical
|Resolution|Wait for the indicated retry duration and retry the operation.

### Base.1.4.SessionLimitExceeded
Session establishment has been requested, but the operation did not complete because the number of simultaneous sessions exceeded the maximum number allowed by the implementation.

| | |
|:---|:---|
|Message Format|"The session establishment did not complete because the number of simultaneous sessions exceeded the maximum number allowed by the implementation."
|Severity|Critical
|Resolution|Before attempting to establish the session, reduce the number of sessions or increase the maximum number of simultaneous sessions allowed (if supported).

### Base.1.4.SessionTerminated
Indicates that the DELETE operation on the Session resource resulted in the successful termination of the session.

| | |
|:---|:---|
|Message Format|"The session was successfully terminated."
|Severity|OK
|Resolution|No resolution is required.

### Base.1.4.SourceDoesNotSupportProtocol
While attempting to access, connect to, or transfer from another location, the other end of the connection did not support the specified protocol.

| | |
|:---|:---|
|Message Format|"The other end of the connection at %1 does not support the specified protocol %2."
|Severity|Critical
|Resolution|Change protocols or URIs. 

### Base.1.4.StringValueTooLong
Indicates that a string value passed to the given resource exceeded its length limit. An example is when a shorter limit is imposed by an implementation than that allowed by the specification.

| | |
|:---|:---|
|Message Format|"The string %1 exceeds the length limit %2."
|Severity|Warning
|Resolution|Resubmit the request with an appropriate string length.

### Base.1.4.Success
The operation completed successfully.

| | |
|:---|:---|
|Message Format|"The operation completed successfully."
|Severity|OK
|Resolution|None

### Base.1.4.UnrecognizedRequestBody
The service detected a request body with malformed JSON.

| | |
|:---|:---|
|Message Format|"The service detected a request body with malformed JSON."
|Severity|Warning
|Resolution|If the operation did not complete, correct the request body and resubmit the request.

### HpeCommon.2.0.ArrayPropertyOutOfBound
The items in the array exceed the maximum  number supported.

| | |
|:---|:---|
|Message Format|"An array %1 was supplied with %2 items that exceeds the maximum supported count of %3."
|Severity|Warning
|Resolution|Retry the operation using the correct number of items for the array.

### HpeCommon.2.0.ConditionalSuccess
A property value was successfully changed but the change may be reverted upon system reset.

| | |
|:---|:---|
|Message Format|"The property %1 was successfully changed to %2, but the change may be reverted upon system reset."
|Severity|Warning
|Resolution|Check the "SettingsResult" messages after the system has reset for errors referring to the corresponding property.

### HpeCommon.2.0.InternalErrorWithParam
The operation was not successful due to an internal service error (shown), but the service is still operational.

| | |
|:---|:---|
|Message Format|"The operation was not successful due to an internal service error (%1), but the service is still operational."
|Severity|Critical
|Resolution|Retry the operation. If the problem persists, consider resetting the service.

### HpeCommon.2.0.InvalidConfigurationSpecified
The specified configuration is not valid.

| | |
|:---|:---|
|Message Format|"The specified configuration is not valid."
|Severity|Warning
|Resolution|Correct the configuration, and then retry the operation.

### HpeCommon.2.0.PropertyValueExceedsMaxLength
The value for the property exceeds the maximum length.

| | |
|:---|:---|
|Message Format|"The value %1 for the property %2 exceeds the maximum length of %3."
|Severity|Warning
|Resolution|Correct the value for the property in the request body, and then retry the operation.

### HpeCommon.2.0.PropertyValueIncompatible
The value for the property is the correct type, but this value is incompatible with the current value of another property.

| | |
|:---|:---|
|Message Format|"The value %1 for the property %2 is incompatible with the value for property %3."
|Severity|Warning
|Resolution|Correct the value for the property in the request body, and then retry the operation.

### HpeCommon.2.0.PropertyValueOutOfRange
The value for the property is out of range.

| | |
|:---|:---|
|Message Format|"The value %1 for the property %2 is out of range %3."
|Severity|Warning
|Resolution|Correct the value for the property in the request body, and then retry the operation.

### HpeCommon.2.0.ResetInProgress
A device or service reset is in progress.

| | |
|:---|:---|
|Message Format|"A reset on %1 is in progress."
|Severity|Warning
|Resolution|Wait for device or service reset to complete, and then retry the operation.

### HpeCommon.2.0.ResetRequired
One or more properties were changed, but these changes will not take effect until the device or service is reset.

| | |
|:---|:---|
|Message Format|"One or more properties were changed, but these changes will not take effect until %1 is reset."
|Severity|Warning
|Resolution|To enable the changed properties, reset the device or service.

### HpeCommon.2.0.ResourceNotReadyRetry
The resource is present but is not ready to perform operations due to an internal condition such as initialization or reset.

| | |
|:---|:---|
|Message Format|"The resource is present but is not ready to perform operations.  The resource will be ready in %1 seconds."
|Severity|Warning
|Resolution|Retry the operation when the resource is ready.

### HpeCommon.2.0.SuccessFeedback
The operation completed successfully

| | |
|:---|:---|
|Message Format|"The operation completed successfully"
|Severity|OK
|Resolution|None

### HpeCommon.2.0.TaskCreated
A task was created in response to the operation.

| | |
|:---|:---|
|Message Format|"A task was created in response to the operation and is accessible at %1."
|Severity|OK
|Resolution|Perform an HTTP GET request on the supplied URI for task status.

### HpeCommon.2.0.UnsupportedHwConfiguration
A previously requested property value change was reverted because the current hardware configuration does not support it.

| | |
|:---|:---|
|Message Format|"The value %1 for property %2 was reverted because the current hardware configuration does not support it."
|Severity|Warning
|Resolution|Ensure that the system's hardware configuration supports the property value.

### iLO.2.13.AHSDisabled
Modifying AHS properties is not possible with AHS disabled.

| | |
|:---|:---|
|Message Format|"Modifying AHS properties is not possible with AHS disabled."
|Severity|Warning
|Resolution|Enable AHS, and then modify the AHS properties.

### iLO.2.13.Accepted
Indicates that one or more properties were correctly changed, but may not be in effect yet.

| | |
|:---|:---|
|Message Format|"Indicates that one or more properties were correctly changed, but may not be in effect yet."
|Severity|OK
|Resolution|None

### iLO.2.13.ActionParameterValueNotInList
Indicates that the correct value type was supplied for the action parameter, but the value is not supported. (The value is not in the enumeration list.)

| | |
|:---|:---|
|Message Format|"The value %1 for the property %2 is not in the list of valid values."
|Severity|Warning
|Resolution|Choose a value from the enumeration list and resubmit the request if the operation failed.

### iLO.2.13.AlertDestinationAssociationError
AlertDestination cannot be configured with both SNMPv1 and SNMPv3.

| | |
|:---|:---|
|Message Format|"AlertDestination cannot be configured with both SNMPv1 and SNMPv3."
|Severity|Warning
|Resolution|For SNMPv1 alert, configure SNMPAlertProtocol to SNMPv1. For SNMPv3 alert, configure SNMPAlertProtocol to SNMPv3.

### iLO.2.13.AlertMailFeatureDisabled
AlertMail feature is disabled.

| | |
|:---|:---|
|Message Format|"AlertMail feature is disabled."
|Severity|Warning
|Resolution|Enable AlertMail feature to send test alert message.

### iLO.2.13.AlreadyInProgress
An operation is already in progress.

| | |
|:---|:---|
|Message Format|"An operation is already in progress."
|Severity|Warning
|Resolution|Wait for the current operation to complete, and then retry the operation.

### iLO.2.13.AlreadyUpToDate
The update did not occur because the component was already up to date.

| | |
|:---|:---|
|Message Format|"The update did not occur because the component was already up to date."
|Severity|Warning
|Resolution|None.

### iLO.2.13.ApmPowerCapModeInUsed
Operation is currently unavailable because the power regulator is set to APM Power Capping Mode.

| | |
|:---|:---|
|Message Format|"Operation is currently unavailable because the power regulator is set to APM Power Capping Mode."
|Severity|Warning
|Resolution|Change the power regulator to other modes rather than APM Power Capping Mode through APM interface.

### iLO.2.13.ArrayPropertyAlreadyExists
Duplicate value.

| | |
|:---|:---|
|Message Format|"The property value %1 is already exists in index %2"
|Severity|Warning
|Resolution|If the operation did not complete, correct the property value in the request body and resubmit the request.

### iLO.2.13.ArrayPropertyOutOfBound
The number of items in the array exceeds the maximum number supported.

| | |
|:---|:---|
|Message Format|"An array %1 was supplied with %2 items that does not meet the minimum supported count of %3 or exceeds the maximum supported count of %4."
|Severity|Warning
|Resolution|Retry the operation using the correct number of items for the array.

### iLO.2.13.ArrayPropertyValueBadParam
The property value is not valid.

| | |
|:---|:---|
|Message Format|"The property value %1 in index %2 is not valid."
|Severity|Warning
|Resolution|Retry the operation using a corrected value.

### iLO.2.13.BatteryBackupUnitSettingsDisabled
Battery Backup Unit settings are currently disabled.

| | |
|:---|:---|
|Message Format|"Battery Backup Unit settings are disabled when the system is configured for Scalable Persistent Memory."
|Severity|Warning
|Resolution|To re-enable Battery Backup Unit settings, disable Scalable Persistent Memory functionality in the system ROM RBSU.

### iLO.2.13.BiosActionTBD
The BIOS action supplied in the POST operation is not yet implemented.

| | |
|:---|:---|
|Message Format|"The BIOS action %1 is not implemented yet."
|Severity|Critical
|Resolution|The action was invalid or the wrong resource was the target. See the implementation documentation for assistance.

### iLO.2.13.BiosPasswordInfoInvalid
The stored BIOS password information is invalid. A system reboot is neccessary to retore password defaults.

| | |
|:---|:---|
|Message Format|"The stored BIOS password information is invalid.  Reboot system."
|Severity|Critical
|Resolution|The system will need to be rebooted to restore BIOS password information to defaults.

### iLO.2.13.BiosPasswordMismatch
The provided OldPassword does not match the stored BIOS password.

| | |
|:---|:---|
|Message Format|"The provided OldPassword does not match the stored BIOS password."
|Severity|Critical
|Resolution|Retry the action with the matching password.

### iLO.2.13.CalibrateInProgress
Power calibrate is in progress.

| | |
|:---|:---|
|Message Format|"Power calibrate is in progress."
|Severity|Warning
|Resolution|Wait for previous power calibrate complete or stop previous power calibrate, and then retry the operation.

### iLO.2.13.CannotRemoveDefaultLanguagePack
Cannot remove default language pack.

| | |
|:---|:---|
|Message Format|"Cannot remove default language pack."
|Severity|Warning
|Resolution|None.

### iLO.2.13.CannotRemoveLanguagePack
Cannot remove language pack.

| | |
|:---|:---|
|Message Format|"Cannot remove %1 language pack."
|Severity|Warning
|Resolution|None.

### iLO.2.13.CannotRemoveLicense
Cannot remove the base license.

| | |
|:---|:---|
|Message Format|"The base license cannot be removed."
|Severity|Warning
|Resolution|None.

### iLO.2.13.ChassisPowerDataUnAvailable
Chassis power regulation data is currently unavailable.

| | |
|:---|:---|
|Message Format|"Chassis power regulation data is currently unavailable."
|Severity|Warning
|Resolution|Reset the management processor or chassis manager, and then retry the operation.

### iLO.2.13.ChassisResetRequired
The chassis properties were correctly changed, but will not take effect until the chassis is reset or all nodes in chassis remain powered off for at least 5 seconds.

| | |
|:---|:---|
|Message Format|"One or more properties were changed and will not take effect until chassis is reset or all nodes in chassis remain powered off for at least 5 seconds."
|Severity|Warning
|Resolution|Reset chassis or remain power off for all nodes in chassis for at least 5 seconds for the settings to take effect.

### iLO.2.13.ComponentUploadAlreadyInProgress
A component upload operation is already in progress.

| | |
|:---|:---|
|Message Format|"A component upload operation is already in progress."
|Severity|Warning
|Resolution|Wait for the current component upload to complete, and then retry the operation.

### iLO.2.13.ComponentUploadFailed
A component upload operation failed.

| | |
|:---|:---|
|Message Format|"A component upload operation failed."
|Severity|Warning
|Resolution|Wait for the current component upload to complete, and then retry the operation.

### iLO.2.13.DailyUpdateLimitExceeded
An update operation failed due to exceeding a daily limit.

| | |
|:---|:---|
|Message Format|"An update operation failed due to exceeding a daily limit."
|Severity|Warning
|Resolution|Retry the operation at a later date.

### iLO.2.13.DemoLicenseKeyPreviouslyInstalled
A license was previously activated and now a demo key may not be used.

| | |
|:---|:---|
|Message Format|"A license was previously activated."
|Severity|Warning
|Resolution|The system is no longer eligible for demo licenses.

### iLO.2.13.DeviceIsBusy
Device was not available for communication.

| | |
|:---|:---|
|Message Format|"Device communication response was busy."
|Severity|Warning
|Resolution|Retry the attempted operation after a delay.

### iLO.2.13.DeviceResetRequired
Indicates that one or more properties were correctly changed, but will not take effect until device is reset.

| | |
|:---|:---|
|Message Format|"One or more properties were changed and will not take effect until the device is reset."
|Severity|Warning
|Resolution|Reset the device for the settings to take effect.

### iLO.2.13.DiagsTestAlreadyRunning
A diagnostics self test is already running.

| | |
|:---|:---|
|Message Format|"A diagnostics self test is already running."
|Severity|Warning
|Resolution|Stop the running test and try again.

### iLO.2.13.DowngradeNotAllowed
The task did not execute because a downgrade is not allowed by policy.

| | |
|:---|:---|
|Message Format|"The task did not execute because a downgrade is not allowed by policy."
|Severity|Warning
|Resolution|Obtain the latest available component and retry, and clear the task from the queue so processing can continue.

### iLO.2.13.DowngradePolicyAlreadySet
The downgrade policy has been set and cannot be changed.

| | |
|:---|:---|
|Message Format|"The downgrade policy has been set and cannot be changed."
|Severity|Warning
|Resolution|None.

### iLO.2.13.ESKMServersNotConfigured
Enterprise Secure Key Manager Servers are not configured.

| | |
|:---|:---|
|Message Format|"Enterprise Secure Key Manager Servers are not configured."
|Severity|OK
|Resolution|None.

### iLO.2.13.ETagTooLong
The supplied ETag is too long. The maximum supported ETag length is 63 bytes.

| | |
|:---|:---|
|Message Format|"The supplied ETag is too long. The maximum supported ETag length is 63 bytes."
|Severity|Warning
|Resolution|Retry the operation using an ETag with a length of 63 bytes or less.

### iLO.2.13.EmptyDNSName
DNS name is empty.

| | |
|:---|:---|
|Message Format|"Empty DNS name."
|Severity|Warning
|Resolution|Retry the request with a valid DNS name.

### iLO.2.13.ErrorIntializingESKM
Failed to initialize ESKM.

| | |
|:---|:---|
|Message Format|"Failed to initialize ESKM."
|Severity|Warning
|Resolution|Check if Account Group, Local CA Certificate Name, Login Name and Password are correct and try again.

### iLO.2.13.EventLogCleared
Event log cleared successfully.

| | |
|:---|:---|
|Message Format|"Event log cleared successfully."
|Severity|OK
|Resolution|None.

### iLO.2.13.EventSubscriptionModified
The event subscription was modified successfully.

| | |
|:---|:---|
|Message Format|"The event subscription was modified successfully."
|Severity|OK
|Resolution|None.

### iLO.2.13.EventSubscriptionRemoved
The event subscription was removed successfully.

| | |
|:---|:---|
|Message Format|"The event subscription was removed successfully."
|Severity|OK
|Resolution|None.

### iLO.2.13.ExtendedInfo
Indicates that extended information is available.

| | |
|:---|:---|
|Message Format|"See @Message.ExtendedInfo for more information."
|Severity|OK
|Resolution|See @Message.ExtendedInfo for more information.

### iLO.2.13.FWFlashSuccessTPMOverrideEnabled
A Trusted Module is  detected in this system. If you have not performed the proper OS encryption procedures, you will lose access to your data if recovery key is not available. Recommended procedure is to suspend encryption software prior to System ROM or Option ROM firmware flash. TPMOverrideFlag is enabled and firmware flash initiated.

| | |
|:---|:---|
|Message Format|"CAUTION: A Trusted Module is detected in this system. Updating the System ROM or Option Card Firmware may have impact to measurements stored in the TM and may have impact to security functionality on the platform which depends on these measurements."
|Severity|OK
|Resolution|None.

### iLO.2.13.FWFlashSuccessTrustedModuleOverrideEnabled
A Trusted Module (type unspecified) is installed in the system and TPMOverrideFlag is enabled. Firmware flash initiated.

| | |
|:---|:---|
|Message Format|"CAUTION: A Trusted Module (type unspecified) has been detected in this system. If you have not performed the proper OS encryption procedures, you will lose access to your data if recovery key is not available. Recommended procedure for Microsoft Windows(R) BitLocker(TM) is to "suspend" BitLocker prior to System ROM or Option ROM firmware flash."
|Severity|OK
|Resolution|None.

### iLO.2.13.FWFlashTPMOverrideFlagRequired
A Trusted Module is  detected in this system. Failure to perform proper OS encryption procedures will result in loss of access to your data if recovery key is not available. Recommended procedure is to suspend encryption software prior to System ROM or Option ROM firmware flash. If you do not have your recovery key or have not suspended encryption software, cancel this firmware upload. Failure to follow these instructions will result in loss of access to your data. To continue with firmware flash TPMOverrideFlag is required.

| | |
|:---|:---|
|Message Format|"CAUTION: A Trusted Module is detected in this system. Updating the System ROM or Option Card Firmware may have impact to measurements stored in the TM and may have impact to security functionality on the platform which depends on these measurements."
|Severity|Warning
|Resolution|Please set the TPMOverrideFlag to true and try again.

### iLO.2.13.FWFlashTrustedModuleOverrideFlagRequired
A Trusted Module (type unspecified) is installed in the system, TPMOverrideFlag is required for firmware flash to proceed.

| | |
|:---|:---|
|Message Format|"CAUTION: A Trusted Module (type unspecified) has been detected in this system. Failure to perform proper OS encryption procedures will result in loss of access to your data if recovery key is not available. Recommended procedure for Microsoft Windows(R) BitLocker(TM) is to "suspend" BitLocker prior to System ROM or Option ROM firmware flash. If you do not have your recovery key or have not suspended BitLocker, exit this flash: Failure to follow these instructions will result in loss of access to your data."
|Severity|Warning
|Resolution|Please set the TPMOverrideFlag to true and try again.

### iLO.2.13.FirmwareFlashAlreadyInProgress
A firmware upgrade operation is already in progress.

| | |
|:---|:---|
|Message Format|"A firmware flash operation is already in progress."
|Severity|Warning
|Resolution|Wait for the current firmware flash to complete, and then retry the operation.

### iLO.2.13.GeneratingCertificate
Generating the X509 Certificate.

| | |
|:---|:---|
|Message Format|"X509 Certificate is being generated and the process might take up to 10 minutes."
|Severity|OK
|Resolution|None.

### iLO.2.13.HardDriveZoneBackupFailure
Backup hard drive zoning configuration to BMC has encountered an error.

| | |
|:---|:---|
|Message Format|"Backup hard drive zoning configuration to BMC has encountered an error."
|Severity|Warning
|Resolution|Retry the operation. If the problem persists, consider resetting the BMC or the entire chassis.

### iLO.2.13.HardDriveZoneFailure
Hard Drive Zoning was in error state.

| | |
|:---|:---|
|Message Format|"Hard Drive Zoning was in error state due to %1."
|Severity|Critical
|Resolution|Retry the operation. If the problem persists, consider resetting the entire chassis.

### iLO.2.13.ICRUInvalidAddress
ICRU returned invalid address for translation.

| | |
|:---|:---|
|Message Format|"ICRU returned invalid address for translation."
|Severity|Warning
|Resolution|Input valid address for translation.

### iLO.2.13.ICRUNotSupported
ICRU feature or function is not supported on the system.

| | |
|:---|:---|
|Message Format|"ICRU feature or function is not supported on the system."
|Severity|Warning
|Resolution|None.

### iLO.2.13.IPv6ConfigurationError
The specified IPv6 configuration caused an error.

| | |
|:---|:---|
|Message Format|"The specified IPv6 configuration was in error due to %1."
|Severity|Warning
|Resolution|Resolve the indicated error in the configuration data.

### iLO.2.13.ImportCertSuccessful
Import Certificate was successful.

| | |
|:---|:---|
|Message Format|"Import Certificate was successful."
|Severity|OK
|Resolution|None.

### iLO.2.13.ImportCertSuccessfuliLOResetinProgress
Import Certificate was successful and the management processor is being reset.

| | |
|:---|:---|
|Message Format|"Import Certificate was successful. Management Processor reset is in progress to enable the new certificate."
|Severity|Warning
|Resolution|None.

### iLO.2.13.ImportCertificateFailed
Failed importing Certificate.

| | |
|:---|:---|
|Message Format|"Failed importing the X509 Certificate."
|Severity|Warning
|Resolution|Retry the operation with proper Certificate information.

### iLO.2.13.ImportSSOParamError
Not a valid parameter.

| | |
|:---|:---|
|Message Format|"Invalid Parameter."
|Severity|Warning
|Resolution|Retry the request with valid parameters.

### iLO.2.13.ImportSSOUriError
Not a valid Uri to import SSO certificate.

| | |
|:---|:---|
|Message Format|"Invalid Uri."
|Severity|Warning
|Resolution|Retry the request with valid URI.

### iLO.2.13.IndicatorLedInvalidStateChange
The request to change the state of the Indicator LED cannot be granted because the current state is either Blinking or is Unknown.

| | |
|:---|:---|
|Message Format|"The Indicator LED cannot be changed when its state is Blinking or Unknown."
|Severity|Warning
|Resolution|Please wait until the server has completed its reserved state.

### iLO.2.13.InstallSetWriteError
The InstallSet write failed.

| | |
|:---|:---|
|Message Format|"The InstallSet write of %1 failed."
|Severity|Warning
|Resolution|Ensure a valid name for the item and that space exists to hold the item.

### iLO.2.13.InterfaceDisabledResetRequired
Disabling one or more interfaces/features will cause certain functionalities to be not available. Please refer to User Guide for details on the implications. Changes will not take effect until the management processor is reset

| | |
|:---|:---|
|Message Format|"CAUTION: Disabling one or more interfaces/features will cause certain functionalities to be not available. Please refer to User Guide for details on the implications. Changes will not take effect until the management processor is reset"
|Severity|OK
|Resolution|None.

### iLO.2.13.InternalErrorWithParam
The operation was not successful due to an internal service error (shown), but the service is still operational.

| | |
|:---|:---|
|Message Format|"The operation was not successful due to an internal service error (%1), but the service is still operational."
|Severity|Critical
|Resolution|Retry the operation. If the problem persists, consider resetting the service.

### iLO.2.13.InvalidConfigurationSpecified
The specified configuration is not valid.

| | |
|:---|:---|
|Message Format|"The specified configuration is not valid."
|Severity|Warning
|Resolution|Correct the configuration, and then retry the operation.

### iLO.2.13.InvalidConfigurationSpecifiedForFederation
iLO Federation Management cannot be supported in the current configuration.

| | |
|:---|:---|
|Message Format|"iLO Federation Management cannot be supported in the current configuration."
|Severity|Warning
|Resolution|Review the management processor network settings or Onboard Administrator settings and refer to the User Guide.

### iLO.2.13.InvalidDwellTime
The dwell time specified is not valid.

| | |
|:---|:---|
|Message Format|"The dwell time %1 is not valid."
|Severity|Warning
|Resolution|Adhere to the dwell time supported.

### iLO.2.13.InvalidEngineID
EngineID should be a hexadecimal number starting with 0x (for example, 0x0102030405abcdef). The string length should be an even number, greater than or equal to 6 characters (excluding the "0x"), and less than or equal to 32 characters.

| | |
|:---|:---|
|Message Format|"EngineID should be a hexadecimal number starting with 0x (for example, 0x0102030405abcdef). The string length should be an even number, greater than or equal to 6 characters (excluding the "0x"), and less than or equal to 32 characters."
|Severity|Warning
|Resolution|Retry the operation using an EngineID within the specified parameters.

### iLO.2.13.InvalidLicenseKey
The license key is not valid.

| | |
|:---|:---|
|Message Format|"The license key is not valid."
|Severity|Warning
|Resolution|Retry the operation using a valid license key.

### iLO.2.13.InvalidOperationForAutoPowerOnState
The operation was not successful because the current auto power on mode specifies power is to remain off.

| | |
|:---|:---|
|Message Format|"The auto power on delay cannot be set because power is configured to remain off."
|Severity|Warning
|Resolution|Verify that the system auto power on mode is set to turn power on or follow the previous power setting.

### iLO.2.13.InvalidOperationForSystemState
The operation was not successful due to the current power state (for example, attempting to turn the power off when it is already off).

| | |
|:---|:---|
|Message Format|"The operation was not successful due to the current power state."
|Severity|Warning
|Resolution|Verify that the system is in the correct power state, and then retry the operation.

### iLO.2.13.InvalidPassphraseLength
The passphrase length is not valid.

| | |
|:---|:---|
|Message Format|"%1 must contain from %2 to %3 characters."
|Severity|Warning
|Resolution|Correct the passphrase, and then retry the operation.

### iLO.2.13.InvalidPasswordComplexity
The password failed the complexity enforcement.

| | |
|:---|:---|
|Message Format|"A valid password must contain three of the following: uppercase, lowercase, numerals, and other."
|Severity|Critical
|Resolution|Retry the operation using a corrected password.

### iLO.2.13.InvalidPasswordLength
The password length is not valid.

| | |
|:---|:---|
|Message Format|"A valid password must contain between %1 to %2 characters."
|Severity|Critical
|Resolution|Retry the operation using a corrected password.

### iLO.2.13.InvalidSerialNumberLength
The serial number length is not valid.

| | |
|:---|:---|
|Message Format|"A valid serial number must be %1 characters of length."
|Severity|Critical
|Resolution|Adjust the length of the serial number and retry the operation.

### iLO.2.13.LicenseKeyDenied
The license key activation was refused.  Includes details.

| | |
|:---|:---|
|Message Format|"The license activation key cannot be installed.  %1"
|Severity|Warning
|Resolution|Address the condition or use a valid license activation key.

### iLO.2.13.LicenseKeyNotSupported
The license key supplied is unsupported on this system.  The key may activate a different product or unsupported tier.

| | |
|:---|:---|
|Message Format|"The supplied license key is not supported on this system."
|Severity|Warning
|Resolution|None.

### iLO.2.13.LicenseKeyRequired
A license key is required to use this operation or feature.

| | |
|:---|:---|
|Message Format|"A license key is required to use this operation or feature."
|Severity|Warning
|Resolution|Install a license key to use this feature.

### iLO.2.13.LoginAttemptDelayed
The login was not successful, so the service enforces a delay before another login is allowed.

| | |
|:---|:---|
|Message Format|"The login was not successful, so the service enforces a delay before another login is allowed."
|Severity|Warning
|Resolution|Wait for the delay time to expire, and then retry the login.

### iLO.2.13.LoginAttemptDelayedSeconds
The login was not successful, so the service enforces a delay before another login is allowed.

| | |
|:---|:---|
|Message Format|"The login was not successful, so the service enforces a %1 second delay before another login is allowed."
|Severity|Warning
|Resolution|None.

### iLO.2.13.MCTPDiscoveryDisabled
Telemetry service and Workload Performance advisor will be not available with MCTP discovery disabled.

| | |
|:---|:---|
|Message Format|"Telemetry service and Workload Performance advisor will be not available with MCTP discovery disabled."
|Severity|Warning
|Resolution|Enable MCTP discovery for Telemetry service and Workload Performance advisor.

### iLO.2.13.MaxProviders
The maximum number of providers are already registered.

| | |
|:---|:---|
|Message Format|"The maximum number of providers are already registered."
|Severity|Warning
|Resolution|None.

### iLO.2.13.MaxVirtualMediaConnectionEstablished
No more Virtual Media connections are available, because the maximum number of connections are already established.

| | |
|:---|:---|
|Message Format|"No more Virtual Media connections are available, because the maximum number of connections are already established."
|Severity|Warning
|Resolution|Close an established Virtual Media connection, and then retry creating or opening another connection.

### iLO.2.13.MembistVariablesNotSupported
Membist variables are not supported on the system.

| | |
|:---|:---|
|Message Format|"Membist variables are not supported on the system."
|Severity|Warning
|Resolution|None.

### iLO.2.13.MemoryInterleaveSetError
The memory set specified in InterleaveSets is not supported.

| | |
|:---|:---|
|Message Format|"The memory set specified in InterleaveSets is not supported."
|Severity|Warning
|Resolution|Ensure the memory set specified in InterleaveSets matches the first set in the memory domain's InterleavableMemrorySets.

### iLO.2.13.NewerVersionRequired
Update does not meet minimum version requirements.

| | |
|:---|:---|
|Message Format|"Update does not meet minimum version requirements."
|Severity|Warning
|Resolution|Use newer version.

### iLO.2.13.NoContent
The requested resource exists but has no content.

| | |
|:---|:---|
|Message Format|"The resource exists but has no content."
|Severity|OK
|Resolution|None

### iLO.2.13.NoEventSubscriptions
There are no event subscriptions registered.

| | |
|:---|:---|
|Message Format|"The operation cannot be completed because there are no event subscribers."
|Severity|Warning
|Resolution|

### iLO.2.13.NoPowerMetering
No support for power metering available on platform.

| | |
|:---|:---|
|Message Format|"No support for power metering available on platform."
|Severity|OK
|Resolution|Enable Power Metering on platform if supported.

### iLO.2.13.NoSNMPAlertDestinationsConfigured
No SNMP alert destinations configured or none of the configured destinations are associated with SNMPv1 protocol or SNMPv3 protocol and user.

| | |
|:---|:---|
|Message Format|"No SNMP alert destinations configured or none of the configured destinations are associated with SNMPv1 protocol or SNMPv3 protocol and user."
|Severity|Warning
|Resolution|Configure at least one SNMP alert destination and associate it with SNMPv1 protocol or SNMPv3 protocol and user.

### iLO.2.13.NoSamples
No power history samples are available.

| | |
|:---|:---|
|Message Format|"No power history samples are available."
|Severity|OK
|Resolution|To accumulate power history samples, power on the server, and then wait at least 5 minutes.

### iLO.2.13.NoScriptedVirtualMediaConnectionAvailable
No scripted virtual media connections exist to perform the operation.

| | |
|:---|:---|
|Message Format|"No scripted virtual media connections exist to perform the operation."
|Severity|Warning
|Resolution|Create or open a scripted virtual media connection, and then retry the operation.

### iLO.2.13.NoSpaceforDNSName
No space to store DNS name.

| | |
|:---|:---|
|Message Format|"No space to store DNS name."
|Severity|Warning
|Resolution|Make sure SSO database has enough space to store DNS name.

### iLO.2.13.NoVirtualMediaConnectionAvailable
No Virtual Media connections exist to perform the operation.

| | |
|:---|:---|
|Message Format|"No Virtual Media connections exist to perform the operation."
|Severity|Warning
|Resolution|Create or open a Virtual Media connection, and then retry the operation.

### iLO.2.13.NodeAssignedCrossRegion
Each zone can only manage the node in the same region, cannot manage overlap region.

| | |
|:---|:---|
|Message Format|"Each zone can only manage the node for range %1 or range %2, cannot manage overlap region."
|Severity|Warning
|Resolution|Correct the out of range value, and then retry the operation.

### iLO.2.13.NodeNotPresentInZone
Operation is currently unavailable because there is no node installed in the zone.

| | |
|:---|:---|
|Message Format|"Operation is currently unavailable because there is no node installed in the zone."
|Severity|Warning
|Resolution|Install at least one node in the zone and retry the operation.

### iLO.2.13.NotSupportedOnNIC
This property is not supported by the indicated network port.

| | |
|:---|:---|
|Message Format|"%1 is not supported on the %2 Network Port."
|Severity|Warning
|Resolution|Do not specify this property on the indicated network port.

### iLO.2.13.NotValidIPAddrOrDNS
The value for the property is not a valid IPv4/v6 address or DNS name.

| | |
|:---|:---|
|Message Format|"The value for property %1 is not a valid IPv4/v6 address or DNS name."
|Severity|Warning
|Resolution|Correct the IPv4/v6 address or DNS name, and then retry the operation.

### iLO.2.13.NotValidIPAddress
The value for the property is not a valid IP address.

| | |
|:---|:---|
|Message Format|"The value %1 is not a valid IP address for %2"
|Severity|Warning
|Resolution|Use a valid IP address.

### iLO.2.13.NotValidSubnetMask
The value for the property is not a valid subnet mask.

| | |
|:---|:---|
|Message Format|"The value %1 is not a valid subnet mask for %2"
|Severity|Warning
|Resolution|Use a valid subnet mask.

### iLO.2.13.OperationAvailableAfterSystemPOST
The value for the property can not be set until System BIOS POST completes.

| | |
|:---|:---|
|Message Format|"Property %1 will be settable after the System BIOS completes POST."
|Severity|Warning
|Resolution|Wait to see the change in value until after the System BIOS completes POST.

### iLO.2.13.OperationWillCompleteAfterSystemPOST
The value for the property will be applied after System BIOS POST completes.

| | |
|:---|:---|
|Message Format|"The value for property %1 will be changed after the System BIOS completes POST."
|Severity|OK
|Resolution|Wait to see the change in value until after the System BIOS completes POST.

### iLO.2.13.PowerCapOACntrld
The enclosure Onboard Administrator is currently managing the power cap.

| | |
|:---|:---|
|Message Format|"The enclosure Onboard Administrator is currently managing the power cap."
|Severity|Warning
|Resolution|Use Onboard Administrator to Manage the PowerCap

### iLO.2.13.PowerCapROMCntrld
The System ROM is currently managing the power cap.

| | |
|:---|:---|
|Message Format|"The System ROM is currently managing the power cap."
|Severity|Warning
|Resolution|Enable RESTful API management of the power cap in System ROM

### iLO.2.13.PowerLimitMayNotTakeEffect
One of power limit setpoint may become unreachable due to power limit range is unknown. It's not recommended configure power limit setpoint when power limit range is unknown.

| | |
|:---|:---|
|Message Format|"One of power limit setpoint may become unreachable due to power limit range is unknown. It's not recommended configure power limit setpoint when power limit range is unknown."
|Severity|Warning
|Resolution|Please execute calibrate action to get power limit range then reconfigure power limit setpoint.

### iLO.2.13.PowerRegulationNotDisable
Operation is currently unavailable because chassis power regulation is enabled.

| | |
|:---|:---|
|Message Format|"Operation is currently unavailable because chassis power regulation is enabled."
|Severity|Warning
|Resolution|Disable chassis power regulation, and then retry the operation.

### iLO.2.13.PowerSettingAdjustRequired
Indicates that one or more power limit setting were correctly changed, but will not take effect until power regulation enable and power regulator mode switch to user configurable mode.

| | |
|:---|:---|
|Message Format|"Indicates that one or more power limit setting were correctly changed, but will not take effect until power regulation enable and power regulator mode switch to user configurable mode."
|Severity|Warning
|Resolution|Enable power regulation and switch power regulator mode to user configurable mode for the settings to take effect.

### iLO.2.13.PowerValueBadParam
The power cap value is not valid.

| | |
|:---|:---|
|Message Format|"The power cap value is not valid."
|Severity|Warning
|Resolution|Retry the operation using a corrected value.

### iLO.2.13.PowerValueInvalidCalibrationData
The request to set the power cap failed. Invalid power cap calibration data. The Power Cap feature is currently unavailable.

| | |
|:---|:---|
|Message Format|"The request to set the power cap failed. Invalid power cap calibration data. The Power Cap feature is currently unavailable"
|Severity|Warning
|Resolution|Restart the server to retrieve calibration data from initial POST.

### iLO.2.13.PowerValueNotOptimal
Power caps set below the specified percentage threshold might become unreachable due to changes in the server. It is recommended to not set a cap for less than this threshold.

| | |
|:---|:---|
|Message Format|"Power caps set below the specified percentage threshold might become unreachable due to changes in the server. It is recommended to not set a cap for less than %1."
|Severity|Warning
|Resolution|Please provide an optimal value in integer considering the power cap range.

### iLO.2.13.PowerValueUnAvailable
Advanced power capping is not currently available due to the system configuration or state.

| | |
|:---|:---|
|Message Format|"Advanced power capping is not currently available due to the system configuration or state."
|Severity|Warning
|Resolution|Change the system configuration or wait for the system to become fully initialized, and then retry the operation.

### iLO.2.13.PowerValueUnSupported
Advanced power capping is not supported on this system.

| | |
|:---|:---|
|Message Format|"Advanced power capping is not supported on this system."
|Severity|Warning
|Resolution|None.

### iLO.2.13.PrimaryESKMServerAccessible
Only the primary ESKM server is accessible.

| | |
|:---|:---|
|Message Format|"No redundancy. Only the primary ESKM server is accessible."
|Severity|OK
|Resolution|None.

### iLO.2.13.PrimarySecondaryAddressesResolveToSameServer
Primary and secondary ESKM server addresses resolve to the same server.

| | |
|:---|:---|
|Message Format|"No redundancy. Primary and secondary ESKM server addresses resolve to the same server."
|Severity|OK
|Resolution|None.

### iLO.2.13.PrimarySecondaryESKMServersAccessible
Both primary and secondary ESKM servers are accessible.

| | |
|:---|:---|
|Message Format|"Redundant solution: Both primary and secondary ESKM servers are accessible."
|Severity|OK
|Resolution|None.

### iLO.2.13.PropertyNotSupported
The property is not supported.

| | |
|:---|:---|
|Message Format|"The property %1 is not supported."
|Severity|Warning
|Resolution|Do not attempt to modify this property.

### iLO.2.13.PropertyNotWritableOrUnknown
The request included a value for a  read-only or unknown property.

| | |
|:---|:---|
|Message Format|"The property %1 is a read-only property and cannot be assigned a value, or not valid for this resource."
|Severity|Warning
|Resolution|If the operation did not complete, remove the property from the request body and resubmit the request.

### iLO.2.13.PropertyValueBadParam
The property value is not valid.

| | |
|:---|:---|
|Message Format|"The property value is not valid."
|Severity|Warning
|Resolution|Retry the operation using a corrected value.

### iLO.2.13.PropertyValueExceedsMaxLength
The value for the property exceeds the maximum length.

| | |
|:---|:---|
|Message Format|"The value %1 for the property %2 exceeds the maximum length of %3."
|Severity|Warning
|Resolution|Correct the value for the property in the request body, and then retry the operation.

### iLO.2.13.PropertyValueIncompatible
The value for the property is the correct type, but this value is incompatible with the current value of another property.

| | |
|:---|:---|
|Message Format|"The value %1 for the property %2 is incompatible with the value for property %3."
|Severity|Warning
|Resolution|Correct the value for the property in the request body, and then retry the operation.

### iLO.2.13.PropertyValueOutOfRange
The value for the property is out of range.

| | |
|:---|:---|
|Message Format|"The value %1 for the property %2 is out of range %3."
|Severity|Warning
|Resolution|Correct the value for the property in the request body, and then retry the operation.

### iLO.2.13.PropertyValueRequired
Indicates that a property was required but not specified.

| | |
|:---|:---|
|Message Format|"%1 requires Property %2 to be specified."
|Severity|Warning
|Resolution|Include the required property in the request body and then retry the operation.

### iLO.2.13.RecoveryInstallSetRequired
A recovery install set is required for this action.

| | |
|:---|:---|
|Message Format|"No recovery install set present."
|Severity|Critical
|Resolution|Create a recovery install set (install set with IsRecovery property set true).

### iLO.2.13.RepairNotSupported
IML event with this severity is not supported to be repaired. IML events with Critical or Warning severities can marked as repaired.

| | |
|:---|:---|
|Message Format|"IML event with %1 severity is not supported to be repaired. IML events with Critical or Warning severities can marked as repaired."
|Severity|Warning
|Resolution|Please do not try to repair IML events with severity other than Critical or Warning.

### iLO.2.13.RequiredPropertyMissing
Indicates that a required property is not specified.

| | |
|:---|:---|
|Message Format|"Required Property %1 needs to be specifed."
|Severity|Warning
|Resolution|Include the required property in the request body and then retry the operation.

### iLO.2.13.ResetInProgress
A management processor reset is in progress.

| | |
|:---|:---|
|Message Format|"A management processor reset is in progress."
|Severity|Warning
|Resolution|Wait for management processor reset to complete, and then retry the operation.

### iLO.2.13.ResetRequired
One or more properties were changed, but these changes will not take effect until the management processor is reset.

| | |
|:---|:---|
|Message Format|"One or more properties were changed, but these changes will not take effect until the management processor is reset."
|Severity|Warning
|Resolution|To enable the changed properties, reset the management processor.

### iLO.2.13.ResourceBeingFlashed
The change to the requested resource failed because the resource is being flashed.

| | |
|:---|:---|
|Message Format|"The change to the requested resource failed because the resource is being flashed."
|Severity|Warning
|Resolution|Retry the operation when the firmware upgrade has completed.

### iLO.2.13.ResourceInUseWithDetail
The change could not be made because the resource was in use or in a transitioning state.

| | |
|:---|:---|
|Message Format|"The change to the resource failed because the resource is in use or in transition."
|Severity|Warning
|Resolution|Retry the request.

### iLO.2.13.ResourceNotReadyRetry
The resource is present but is not ready to perform operations due to an internal condition such as initialization or reset.

| | |
|:---|:---|
|Message Format|"The resource is present but is not ready to perform operations.  The resource will be ready in %1 seconds."
|Severity|Warning
|Resolution|Retry the operation when the resource is ready.

### iLO.2.13.ResourceTemporarilyUnavailable
The resource is temporarily unavailable because the firmware is being flashed.

| | |
|:---|:---|
|Message Format|"The resource is temporarily unavailable because the firmware is being flashed."
|Severity|Warning
|Resolution|Retry the operation when the firmware upgrade has completed.

### iLO.2.13.SMBIOSRecordNotFound
The SMBIOS record type is not found or is not supported on the system.

| | |
|:---|:---|
|Message Format|"The SMBIOS record type %1 is not found or is not supported on the system."
|Severity|Warning
|Resolution|Reset the system to update the SMBIOS records. If the problem persists then the SMBIOS record type is not supported.

### iLO.2.13.SNMPAlertDisabled
The operation could not be completed because SNMP alerts are disabled.

| | |
|:---|:---|
|Message Format|"The operation could not be completed because SNMP alerts are disabled."
|Severity|Warning
|Resolution|Enable SNMP alerts and retry the operation.

### iLO.2.13.SNMPDisabled
Modifying SNMP properties is not possible with SNMP disabled.

| | |
|:---|:---|
|Message Format|"Modifying SNMP properties is not possible with SNMP disabled."
|Severity|Warning
|Resolution|Enable SNMP, and then modify the SNMP properties.

### iLO.2.13.SNMPTestAlertFailed
The SNMP Test Alert did not send successfully.

| | |
|:---|:---|
|Message Format|"The SNMP Test Alert did not send successfully."
|Severity|Warning
|Resolution|Verify the test alert content and retry.

### iLO.2.13.SNTPConfigurationManagedByDHCPAndIsReadOnly
SNTP configuration is currently managed by DHCP and is therefore read-only.

| | |
|:---|:---|
|Message Format|"%1 cannot be changed while DHCP is configured to provide SNTP settings."
|Severity|Warning
|Resolution|Disable SNTP configuration options in both DHCPv4 and DHCPv6 (see /Managers/n/NICs), and then reconfigure SNTP as desired with static settings.

### iLO.2.13.SSOCertficateEmpty
SSO Certificate is Empty.

| | |
|:---|:---|
|Message Format|"Empty SSO Certificate."
|Severity|Warning
|Resolution|None.

### iLO.2.13.SSOCertificateReadError
SSO Certificate Read Error.

| | |
|:---|:---|
|Message Format|"Error reading SSO certificate."
|Severity|Warning
|Resolution|Retry the request with valid SSO certificate.

### iLO.2.13.SSONoSpaceError
No space to store SSO certificate.

| | |
|:---|:---|
|Message Format|"No space to store SSO certificate."
|Severity|Warning
|Resolution|Make sure SSO database has enough space to store SSO certificate.

### iLO.2.13.SSORecordNotFound
SSO Record Not Found.

| | |
|:---|:---|
|Message Format|"SSO Record Not Found."
|Severity|Warning
|Resolution|None.

### iLO.2.13.SamplesNotCaptured
Samples are not captured for %1 duration.

| | |
|:---|:---|
|Message Format|"Samples for metrics are not captured for %1 duration."
|Severity|OK
|Resolution|Wait for the current duration to complete, and then retry.

### iLO.2.13.SecondaryESKMServerAccessible
Only the secondary ESKM server is accessible.

| | |
|:---|:---|
|Message Format|"No redundancy. Only the secondary ESKM server is accessible."
|Severity|OK
|Resolution|None.

### iLO.2.13.ServerConfigLockStatusUnknown
The current status of Server Configuration Lock is unknown.

| | |
|:---|:---|
|Message Format|"The current status of Server Configuration Lock is unknown."
|Severity|Warning
|Resolution|Ensure if the BIOS firmware supports Server Configuration Lock. If supported, reboot the server and retry the operation

### iLO.2.13.ServerConfigurationLockEnabled
Server Configuration Lock is enabled.

| | |
|:---|:---|
|Message Format|"Server Configuration Lock is enabled."
|Severity|Warning
|Resolution|Disable Server Configuration Lock to initiate secure erase of the system

### iLO.2.13.SuccessFeedback
The operation completed successfully.

| | |
|:---|:---|
|Message Format|"The operation completed successfully."
|Severity|OK
|Resolution|None

### iLO.2.13.SyslogFeatureDisabled
Remote Syslog feature is disabled.

| | |
|:---|:---|
|Message Format|"Remote syslog feature is disabled."
|Severity|Warning
|Resolution|Enable remote syslog feature to send test syslog message.

### iLO.2.13.SystemPowerOffRequired
To perform this operation, power off the system. AutoPowerOn must be set to achieve a power restore.

| | |
|:---|:---|
|Message Format|"To perform this operation, power off the system."
|Severity|OK
|Resolution|To perform this operation, power off the system.

### iLO.2.13.SystemPowerStateChangeFailed
System power state change failed (for example, attempting to turn the system power On/Off failed)

| | |
|:---|:---|
|Message Format|"System power state change failed"
|Severity|Warning
|Resolution|Retry the request.

### iLO.2.13.SystemResetRequired
The system properties were correctly changed, but will not take effect until the system is reset.

| | |
|:---|:---|
|Message Format|"One or more properties were changed and will not take effect until system is reset."
|Severity|Warning
|Resolution|Reset system for the settings to take effect.

### iLO.2.13.TokenRequired
Proper 'X-HPRESTFULAPI-AuthToken' authorization token not provided.

| | |
|:---|:---|
|Message Format|"Proper 'X-HPRESTFULAPI-AuthToken' authorization token not provided."
|Severity|Critical
|Resolution|Create proper 'X-HPRESTFULAPI-AuthToken' authorization token. Send token in using the proper HTTP header.

### iLO.2.13.UnableModifyRights
Unable to modify user rights.

| | |
|:---|:---|
|Message Format|"Unable to modify user rights."
|Severity|Warning
|Resolution|None.

### iLO.2.13.UnableToModifyAfterVirtualMediaInsert
The value for the property cannot be changed after virual media image is inserted.

| | |
|:---|:---|
|Message Format|"The value for property %1 cannot be changed after virual media image is inserted."
|Severity|Warning
|Resolution|Retry the operation during virtual media image inseration.

### iLO.2.13.UnableToModifyDueToMissingComponent
The value for the property cannot be changed because a related hardware component is not installed.

| | |
|:---|:---|
|Message Format|"The value for property %1 cannot be changed because a related hardware component is not installed."
|Severity|Warning
|Resolution|Install the hardware component and retry the operation.

### iLO.2.13.UnableToModifyDuringSystemPOST
The value for the property cannot be changed while the computer system BIOS is in POST.

| | |
|:---|:---|
|Message Format|"The value for property %1 cannot be changed while the computer system BIOS is in POST."
|Severity|Warning
|Resolution|After the computer system is either fully booted or powered off, retry the operation.

### iLO.2.13.UnauthorizedLoginAttempt
The login was not successful, because the supplied credentials could not be authorized.

| | |
|:---|:---|
|Message Format|"The login was not successful, because the supplied credentials could not be authorized."
|Severity|Warning
|Resolution|Log in with authorized user name and password credentials.

### iLO.2.13.UnsupportedCipherAlgo
Incompatible Cipher Algorithm in FIPS or CNSA Mode.

| | |
|:---|:---|
|Message Format|"Incompatible Cipher Algorithm %1 in %2 Mode."
|Severity|Warning
|Resolution|Select compatible Cipher Algorithm.

### iLO.2.13.UnsupportedOperation
This operation is not supported by RIS for the current system.

| | |
|:---|:---|
|Message Format|"This operation is not supported by RIS for the current system."
|Severity|Warning
|Resolution|None.

### iLO.2.13.UnsupportedOperationInChassisVersion
This operation is not supported by the current version of the XL Chassis firmware.

| | |
|:---|:---|
|Message Format|"This operation is not supported by the current version of the XL Chassis firmware."
|Severity|Warning
|Resolution|Please update the XL Chassis firmware to latest version.

### iLO.2.13.UnsupportedOperationInLegacyBootMode
This operation is not supported when the system Boot Mode is set to Legacy BIOS.

| | |
|:---|:---|
|Message Format|" This operation is not supported when the system Boot Mode is set to Legacy BIOS."
|Severity|Warning
|Resolution|Change the Boot Mode to UEFI and retry the operation.

### iLO.2.13.UnsupportedOperationInSystemBIOS
This operation is not supported by the current version of the system BIOS.

| | |
|:---|:---|
|Message Format|"This operation is not supported by the current version of the system BIOS."
|Severity|Warning
|Resolution|None.

### iLO.2.13.UnsupportedSecurityState
The operation was not successful due to the current security state of the management processor.

| | |
|:---|:---|
|Message Format|"The operation was not successful due to the current security state of the management processor."
|Severity|Warning
|Resolution|Retry the operation with the correct security state.

### iLO.2.13.UpdateBadParameter
The update failed because a bad parameter was supplied.

| | |
|:---|:---|
|Message Format|"The update failed because a bad parameter was supplied."
|Severity|Critical
|Resolution|Supply correct parameters to the component and retry the update.

### iLO.2.13.UpdateCancelled
The update was canceled by the update process.

| | |
|:---|:---|
|Message Format|"The update was canceled by the update process."
|Severity|Critical
|Resolution|Retry the update.

### iLO.2.13.UpdateDependencyFailure
The update did not complete because the component failed a dependency check.

| | |
|:---|:---|
|Message Format|"The update did not complete because the component failed a dependency check."
|Severity|Critical
|Resolution|Install any dependent components first and then retry this update.

### iLO.2.13.UpdateFailed
The update failed with a component specific error (%1).

| | |
|:---|:---|
|Message Format|"The update failed with a component specific error (%1)."
|Severity|Critical
|Resolution|Retry the update after remedying the component error.

### iLO.2.13.UpdateInPOST
System must not be booted past POST in order to perform this update

| | |
|:---|:---|
|Message Format|"System must not be booted past POST in order to perform this update"
|Severity|Critical
|Resolution|Boot to UEFI and retry the update.

### iLO.2.13.UpdateInterrupted
The update was interrupted.

| | |
|:---|:---|
|Message Format|"The update was interrupted."
|Severity|Critical
|Resolution|Retry the update.

### iLO.2.13.UpdateInvalidFile
The update operation failed because the file is not valid.

| | |
|:---|:---|
|Message Format|"The update operation failed because the file is not valid."
|Severity|Critical
|Resolution|Remove and re-add the component to the repository and try the operation again.

### iLO.2.13.UpdateInvalidOS
The update did not occur because the running OS is not valid.

| | |
|:---|:---|
|Message Format|"The update did not occur because the running OS is not valid."
|Severity|Critical
|Resolution|Retry the update while running the correct OS.

### iLO.2.13.UpdateNotApplicable
The task was not completed because the component was not applicable to this system.

| | |
|:---|:---|
|Message Format|"The task was not completed because the component was not applicable to this system."
|Severity|Critical
|Resolution|None.

### iLO.2.13.UpdateRepositoryUnavailable
The update operation failed because the component repository is unavailable.

| | |
|:---|:---|
|Message Format|"The update operation failed because the component repository is unavailable."
|Severity|Critical
|Resolution|None.

### iLO.2.13.UpdateTaskQueueFull
The Invoke action was not successful because the update task queue is full.

| | |
|:---|:---|
|Message Format|"The Invoke action was not successful because the update task queue is full."
|Severity|Critical
|Resolution|Remove completed tasks from the update task queue to retry the operation.

### iLO.2.13.UpdateTaskQueueWriteError
The UpdateTaskQueue write failed.

| | |
|:---|:---|
|Message Format|"The UpdateTaskQueue write of %1 failed."
|Severity|Warning
|Resolution|Ensure a valid name for the item and that space exists to hold the item.

### iLO.2.13.UpdateTemporarilyUnavailable
The system is temporarily unable to perform this update

| | |
|:---|:---|
|Message Format|"The system is temporarily unable to perform this update"
|Severity|Critical
|Resolution|Retry the update, ensuring that power state is stable.

### iLO.2.13.UpdateWithPowerOff
System power must be off to perform this update

| | |
|:---|:---|
|Message Format|"System power must be off to perform this update"
|Severity|Critical
|Resolution|Power system on and retry the update.

### iLO.2.13.UpdateWithPowerOn
System power must be on to perform this update

| | |
|:---|:---|
|Message Format|"System power must be on to perform this update"
|Severity|Critical
|Resolution|Power system on and retry the update.

### iLO.2.13.UserAlreadyExist
The user or login user name already exists.

| | |
|:---|:---|
|Message Format|"The user or login user name already exists."
|Severity|Warning
|Resolution|Try a different user or login user name.

### iLO.2.13.UserNameAlreadyExists
Duplicate SNMPv3 User.

| | |
|:---|:---|
|Message Format|"The username %1 already exists in the list"
|Severity|Warning
|Resolution|Enter a different name and try again.

### iLO.2.13.VirtualMediaIsDisabled
Virtual Media has been disabled.

| | |
|:---|:---|
|Message Format|"Virtual Media has been disabled."
|Severity|Warning
|Resolution|Enable Virtual Media to perform this operation.

### iLO.2.13.ZonePowerLimitExceeded
The sum of zone power limit cannot be more than chassis power limit.

| | |
|:---|:---|
|Message Format|"The value %1 for the sum of %2 cannot be more than chassis power limit %3."
|Severity|Warning
|Resolution|Correct the value avoid the sum of power limit exceeds chassis power limit, and then retry the operation.

### iLO.2.13.iLOResetAndSystemRebootRequired
Indicates that one or more properties were correctly changed, but will not take effect until device is reset and system is rebooted.

| | |
|:---|:---|
|Message Format|"One or more properties were changed and will not take effect until the device is reset and system is rebooted"
|Severity|Warning
|Resolution|Reset the management processor and reboot the server.

### iLO.2.13.iLOSubnetConflict
The subnet being configured has conflicts.

| | |
|:---|:---|
|Message Format|"The subnet being configured for %1 conflicts with %2."
|Severity|Warning
|Resolution|Configure this interface with a different IP Address or Subnet Mask.

### iLO.2.13.iLOVirtualNICDisabled
The Virtual NIC is disabled.

| | |
|:---|:---|
|Message Format|"The Virtual NIC is disabled."
|Severity|Warning
|Resolution|Enable iLO Virtual NIC to perform this operation.

### TaskEvent.1.0.TaskAborted
The task with id %1 has been aborted.

| | |
|:---|:---|
|Message Format|"The task with id %1 has been aborted."
|Severity|Critical
|Resolution|None.

### TaskEvent.1.0.TaskCancelled
The task with id %1 has been cancelled.

| | |
|:---|:---|
|Message Format|"The task with id %1 has been cancelled."
|Severity|Warning
|Resolution|None.

### TaskEvent.1.0.TaskCompletedOK
The task with id %1 has completed.

| | |
|:---|:---|
|Message Format|"The task with id %1 has completed."
|Severity|OK
|Resolution|None.

### TaskEvent.1.0.TaskCompletedWarning
The task with id %1 has completed with warnings.

| | |
|:---|:---|
|Message Format|"The task with id %1 has completed with warnings."
|Severity|Warning
|Resolution|None.

### TaskEvent.1.0.TaskPaused
The task with id %1 has been paused.

| | |
|:---|:---|
|Message Format|"The task with id %1 has been paused."
|Severity|Warning
|Resolution|None.

### TaskEvent.1.0.TaskProgessChanged
The task with id %1 has changed to progress %2 percent complete.

| | |
|:---|:---|
|Message Format|"The task with id %1 has changed to progress %2 percent complete."
|Severity|OK
|Resolution|None.

### TaskEvent.1.0.TaskRemoved
The task with id %1 has been removed.

| | |
|:---|:---|
|Message Format|"The task with id %1 has been removed."
|Severity|Warning
|Resolution|None.

### TaskEvent.1.0.TaskResumed
The task with id %1 has been resumed.

| | |
|:---|:---|
|Message Format|"The task with id %1 has been resumed."
|Severity|OK
|Resolution|None.

### TaskEvent.1.0.TaskStarted
The task with id %1 has started.

| | |
|:---|:---|
|Message Format|"The task with id %1 has started."
|Severity|OK
|Resolution|None.
