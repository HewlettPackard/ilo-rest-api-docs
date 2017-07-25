### Base.AccessDenied

**Description:**  While attempting to access, connect to, or transfer to/from another resource, the service was denied access.

|   |   |
|:---|:---|
|Message Format|"While attempting to establish a connection to %1, the service was denied access."
|Severity|Critical
|Resolution|Verify that the URI is correct and that the service has the appropriate credentials.

### Base.AccountForSessionNoLongerExists

**Description:**  The account for current session is removed and the current session is also removed.

|   |   |
|:---|:---|
|Message Format|"The account for the session is removed and the current session is also removed."
|Severity|OK
|Resolution|Attempt to connect using a valid account.

### Base.AccountModified

**Description:**  The account was modified successfully.

|   |   |
|:---|:---|
|Message Format|"The account was modified successfully."
|Severity|OK
|Resolution|None.

### Base.AccountNotModified

**Description:**  The request was unable to modify the account.

|   |   |
|:---|:---|
|Message Format|"The account modification request did not complete."
|Severity|Warning
|Resolution|If the operation did not complete, check the authorization or the request body for issues and resubmit the request.

### Base.AccountRemoved

**Description:**  The account was removed successfully.

|   |   |
|:---|:---|
|Message Format|"The account was removed successfully."
|Severity|OK
|Resolution|None.

### Base.ActionNotSupported

**Description:**  The action supplied in the POST operation is not supported by the resource.

|   |   |
|:---|:---|
|Message Format|"The action %1 is not supported by the resource."
|Severity|Critical
|Resolution|The action was invalid or the wrong resource was the target. See the implementation documentation for assistance.

### Base.ActionParameterDuplicate

**Description:**  The action was submitted with a duplicate parameter in the request body.

|   |   |
|:---|:---|
|Message Format|"The action %1 was submitted with more than one value for the parameter %2."
|Severity|Warning
|Resolution|Resubmit the action with only one instance of the parameter in the request body.

### Base.ActionParameterMissing

**Description:**  The requested action is missing a parameter that is required to process the action.

|   |   |
|:---|:---|
|Message Format|"The action %1 requires that the parameter %2 be present in the request body."
|Severity|Critical
|Resolution|Resubmit the action with the required parameter in the request body.

### Base.ActionParameterNotSupported

**Description:**  The action parameter is not supported on the target resource.

|   |   |
|:---|:---|
|Message Format|"The parameter %1 for the action %2 is not supported on the target resource."
|Severity|Warning
|Resolution|If the operation did not complete, remove the parameter and resubmit the request.

### Base.ActionParameterUnknown

**Description:**  An action was submitted, but a supplied parameter did not match any of the known parameters.

|   |   |
|:---|:---|
|Message Format|"The action %1 was submitted with the invalid parameter %2."
|Severity|Warning
|Resolution|If the operation did not complete, correct the invalid parameter and resubmit the request.

### Base.ActionParameterValueFormatError

**Description:**  The value type is correct, but the format is not supported or the size/length is exceeded

|   |   |
|:---|:---|
|Message Format|"The value %1 for the parameter %2 in the action %3 is in a format that is not supported by the parameter."
|Severity|Warning
|Resolution|If the operation did not complete, correct the parameter value in the request body and resubmit the request.

### Base.ActionParameterValueTypeError

**Description:**  The parameter contains an incorrect value type. For example, a number value for a string parameter type.

|   |   |
|:---|:---|
|Message Format|"The value %1 for the parameter %2 in the action %3 is the incorrect parameter type."
|Severity|Warning
|Resolution|If the operation did not complete, correct the parameter value in the request body and resubmit the request.

### Base.CouldNotEstablishConnection

**Description:**  An attempt to access the resource, image, or file at the URI was unsuccessful because a session could not be established.

|   |   |
|:---|:---|
|Message Format|"The service was unable to establish a connection with the URI %1."
|Severity|Critical
|Resolution|Verify that the URI contains a valid and reachable node name, protocol information, and other URI components.

### Base.CreateFailedMissingReqProperties

**Description:**  A create operation was attempted on a resource, but a required property was missing from the request.

|   |   |
|:---|:---|
|Message Format|"The create operation did not complete because the required property %1 was missing from the request."
|Severity|Critical
|Resolution|If the operation did not complete, include the required property with a valid value in the request body and resubmit the request.

### Base.CreateLimitReachedForResource

**Description:**  No more resources can be created.

|   |   |
|:---|:---|
|Message Format|"No more resources can be created."
|Severity|Critical
|Resolution|If the operation did not complete, delete resources and resubmit the request.

### Base.Created

**Description:**  The resource has been created successfully.

|   |   |
|:---|:---|
|Message Format|"The resource has been created successfully."
|Severity|OK
|Resolution|None

### Base.EventSubscriptionLimitExceeded

**Description:**  The event subscription establishment has been requested, but the operation did not complete because the number of simultaneous subscriptions exceeded the maximum number allowed by the implementation.

|   |   |
|:---|:---|
|Message Format|"The event subscription did not complete because the number of simultaneous subscriptions exceeded the maximum number allowed by the implementation."
|Severity|Critical
|Resolution|Before attempting to establish the event subscription, reduce the number of subscriptions or increase the maximum number of simultaneous subscriptions allowed (if supported).

### Base.InsufficientPrivilege

**Description:**  The account or credentials associated with the current session are not authorized to perform the requested operation.

|   |   |
|:---|:---|
|Message Format|"The account or credentials associated with the current session are not authorized to perform the requested operation."
|Severity|Critical
|Resolution|Retry the operation with an authorized account or credentials.

### Base.InternalError

**Description:**  The request did not complete due to an unknown internal error, but the service is still operational.

|   |   |
|:---|:---|
|Message Format|"The request failed due to an internal service error, but the service is still operational."
|Severity|Critical
|Resolution|Resubmit the request. If the problem persists, consider resetting the service.

### Base.InvalidObject

**Description:**  The object is not valid.

|   |   |
|:---|:---|
|Message Format|"The object at %1 is not valid."
|Severity|Critical
|Resolution|If the operation did not complete, the object is malformed or the URI is incorrect. Make the appropriate corrections and resubmit the request.

### Base.MalformedJSON

**Description:**  The request body contains malformed JSON.

|   |   |
|:---|:---|
|Message Format|"The request body submitted is malformed JSON and cannot be parsed by the receiving service."
|Severity|Critical
|Resolution|Verify that the request body is valid JSON and resubmit the request.

### Base.NoValidSession

**Description:**  The operation did not complete because a valid session is required in order to access resources.

|   |   |
|:---|:---|
|Message Format|"There is no valid session established with the implementation."
|Severity|Critical
|Resolution|Establish a session before attempting any operations.

### Base.PropertyDuplicate

**Description:**  A duplicate property is in the request body.

|   |   |
|:---|:---|
|Message Format|"The property %1 is duplicated in the request."
|Severity|Warning
|Resolution|If the operation did not complete, remove the duplicate property from the request body and resubmit the request.

### Base.PropertyMissing

**Description:**  The request does not include a required property.

|   |   |
|:---|:---|
|Message Format|"The property %1 is a required property and must be included in the request."
|Severity|Warning
|Resolution|If the operation did not complete, verify the property is in the request body and has a valid value.

### Base.PropertyNotWritable

**Description:**  The request included a value for a read-only property.

|   |   |
|:---|:---|
|Message Format|"The property %1 is a read-only property and cannot be assigned a value."
|Severity|Warning
|Resolution|If the operation did not complete, remove the property from the request body and resubmit the request.

### Base.PropertyUnknown

**Description:**  An unknown property is in the request body.

|   |   |
|:---|:---|
|Message Format|"The property %1 is not valid for this resource."
|Severity|Warning
|Resolution|If the operation did not complete, remove the unknown property from the request body and resubmit the request.

### Base.PropertyValueFormatError

**Description:**  The value type is correct, but the format is not supported or the size/length is exceeded.

|   |   |
|:---|:---|
|Message Format|"The value %1 for the property %2 is in a format that is not supported by the property."
|Severity|Warning
|Resolution|If the operation did not complete, correct the property value in the request body and resubmit the request.

### Base.PropertyValueNotInList

**Description:**  The value type is correct, but the value is not supported.

|   |   |
|:---|:---|
|Message Format|"The value %1 for the property %2 is not valid."
|Severity|Warning
|Resolution|If the operation did not complete, choose a value from the enumeration list and resubmit your request.

### Base.PropertyValueTypeError

**Description:**  The property value contains an incorrect property type. For example, a number value for a string property type.

|   |   |
|:---|:---|
|Message Format|"The value %1 for the property %2 is the incorrect property type."
|Severity|Warning
|Resolution|If the operation did not complete, correct the property value in the request body and resubmit the request.

### Base.QueryNotSupported

**Description:**  The query is not supported by the implementation.

|   |   |
|:---|:---|
|Message Format|"Querying is not supported by the implementation."
|Severity|Warning
|Resolution|If the operation did not complete, remove the query parameter and resubmit the request.

### Base.QueryNotSupportedOnResource

**Description:**  The query is not supported on the resource. For example, a start/count query is attempted on a resource that is not a collection.

|   |   |
|:---|:---|
|Message Format|"Querying is not supported on the requested resource."
|Severity|Warning
|Resolution|If the operation did not complete, remove the query parameters and resubmit the request.

### Base.QueryParameterOutOfRange

**Description:**  The query parameter value is out of range for the resource. For example, a page is requested that is outside the valid page range.

|   |   |
|:---|:---|
|Message Format|"The value %1 for the query parameter %2 is out of range %3."
|Severity|Warning
|Resolution|Specify a query parameter value that is within range. For example, a page that is within the valid range of pages.

### Base.QueryParameterValueFormatError

**Description:**  The value type is correct, but the format is not supported or the size/length was exceeded.

|   |   |
|:---|:---|
|Message Format|"The value %1 for the parameter %2 is in a format that is not supported by the parameter."
|Severity|Warning
|Resolution|If the operation did not complete, correct the value for the query parameter in the request body and resubmit the request.

### Base.QueryParameterValueTypeError

**Description:**  The query parameter contains an incorrect value type. For example, a number supplied for a query parameter that requires a string.

|   |   |
|:---|:---|
|Message Format|"The value %1 for the query parameter %2 is the incorrect type of value for the query parameter."
|Severity|Warning
|Resolution|If the operation did not complete, correct the value for the query parameter in the request body and resubmit the request.

### Base.ResourceAlreadyExists

**Description:**  The create resource operation did not complete because the resource already exists.

|   |   |
|:---|:---|
|Message Format|"The requested resource already exists."
|Severity|Critical
|Resolution|Do not attempt the create operation because the resource already exists.

### Base.ResourceAtUriInUnknownFormat

**Description:**  The URI is valid, but the resource or image at that URI is in a format that is not supported by the service.

|   |   |
|:---|:---|
|Message Format|"The resource at %1 is in a format that is not supported by the service."
|Severity|Critical
|Resolution|Place a resource, image, or file that is supported by the service at the URI.

### Base.ResourceAtUriUnauthorized

**Description:**  An attempt to access the resource, image, or file at the URI is unauthorized.

|   |   |
|:---|:---|
|Message Format|"While accessing the resource at %1, the service received an authorization error %2."
|Severity|Critical
|Resolution|Verify that the appropriate access is provided for the service to access the URI.

### Base.ResourceCannotBeDeleted

**Description:**  A delete operation was attempted on a resource that cannot be deleted.

|   |   |
|:---|:---|
|Message Format|"The delete request did not complete because the resource cannot be deleted."
|Severity|Critical
|Resolution|Do not attempt to delete a resource that does not support the REST API DELETE operation.

### Base.ResourceInUse

**Description:**  The request to change the resource was rejected because the resource was in use or in transition.

|   |   |
|:---|:---|
|Message Format|"The change to the resource did not complete because the resource is in use or in transition."
|Severity|Warning
|Resolution|If the operation did not complete, wait until the resource is free and resubmit the request.

### Base.ResourceMissingAtURI

**Description:**  The operation expected an image or resource at the provided URI, but found none.

|   |   |
|:---|:---|
|Message Format|"The resource at the URI %1 was not found."
|Severity|Critical
|Resolution|Place a valid resource at the URI or correct the URI and resubmit the request.

### Base.ServiceInUnknownState

**Description:**  The operation did not complete because the service is in an unknown state and cannot take incoming requests.

|   |   |
|:---|:---|
|Message Format|"The operation did not complete because the service is in an unknown state and cannot take incoming requests."
|Severity|Critical
|Resolution|If the operation did not complete, restart the service and resubmit the request.

### Base.ServiceShuttingDown

**Description:**  The operation did not complete because the service is shutting down.

|   |   |
|:---|:---|
|Message Format|"The operation did not complete because the service is shutting down and cannot take incoming requests."
|Severity|Critical
|Resolution|If the operation did not complete, resubmit the request when the service is available.

### Base.ServiceTemporarilyUnavailable

**Description:**  The service is temporarily unavailable.

|   |   |
|:---|:---|
|Message Format|"The service is temporarily unavailable.  Retry in %1 seconds."
|Severity|Critical
|Resolution|Wait for the indicated retry duration and retry the operation.

### Base.SessionLimitExceeded

**Description:**  Session establishment has been requested, but the operation did not complete because the number of simultaneous sessions exceeded the maximum number allowed by the implementation.

|   |   |
|:---|:---|
|Message Format|"The session establishment did not complete because the number of simultaneous sessions exceeded the maximum number allowed by the implementation."
|Severity|Critical
|Resolution|Before attempting to establish the session, reduce the number of sessions or increase the maximum number of simultaneous sessions allowed (if supported).

### Base.SourceDoesNotSupportProtocol

**Description:**  While attempting to access, connect to, or transfer from another location, the other end of the connection did not support the specified protocol.

|   |   |
|:---|:---|
|Message Format|"The other end of the connection at %1 does not support the specified protocol %2."
|Severity|Critical
|Resolution|Change protocols or URIs. 

### Base.Success

**Description:**  The operation completed successfully.

|   |   |
|:---|:---|
|Message Format|"The operation completed successfully."
|Severity|OK
|Resolution|None

### Base.UnrecognizedRequestBody

**Description:**  The service detected a request body with malformed JSON.

|   |   |
|:---|:---|
|Message Format|"The service detected a request body with malformed JSON."
|Severity|Warning
|Resolution|If the operation did not complete, correct the request body and resubmit the request.

### HpeCommon.ArrayPropertyOutOfBound

**Description:**  The items in the array exceed the maximum  number supported.

|   |   |
|:---|:---|
|Message Format|"An array %1 was supplied with %2 items that exceeds the maximum supported count of %3."
|Severity|Warning
|Resolution|Retry the operation using the correct number of items for the array.

### HpeCommon.ConditionalSuccess

**Description:**  A property value was successfully changed but the change may be reverted upon system reset.

|   |   |
|:---|:---|
|Message Format|"The property %1 was successfully changed to %2, but the change may be reverted upon system reset."
|Severity|Warning
|Resolution|Check the "SettingsResult" messages after the system has reset for errors referring to the corresponding property.

### HpeCommon.InternalErrorWithParam

**Description:**  The operation was not successful due to an internal service error (shown), but the service is still operational.

|   |   |
|:---|:---|
|Message Format|"The operation was not successful due to an internal service error (%1), but the service is still operational."
|Severity|Critical
|Resolution|Retry the operation. If the problem persists, consider resetting the service.

### HpeCommon.InvalidConfigurationSpecified

**Description:**  The specified configuration is not valid.

|   |   |
|:---|:---|
|Message Format|"The specified configuration is not valid."
|Severity|Warning
|Resolution|Correct the configuration, and then retry the operation.

### HpeCommon.PropertyValueExceedsMaxLength

**Description:**  The value for the property exceeds the maximum length.

|   |   |
|:---|:---|
|Message Format|"The value %1 for the property %2 exceeds the maximum length of %3."
|Severity|Warning
|Resolution|Correct the value for the property in the request body, and then retry the operation.

### HpeCommon.PropertyValueIncompatible

**Description:**  The value for the property is the correct type, but this value is incompatible with the current value of another property.

|   |   |
|:---|:---|
|Message Format|"The value %1 for the property %2 is incompatible with the value for property %3."
|Severity|Warning
|Resolution|Correct the value for the property in the request body, and then retry the operation.

### HpeCommon.PropertyValueOutOfRange

**Description:**  The value for the property is out of range.

|   |   |
|:---|:---|
|Message Format|"The value %1 for the property %2 is out of range %3."
|Severity|Warning
|Resolution|Correct the value for the property in the request body, and then retry the operation.

### HpeCommon.ResetInProgress

**Description:**  A device or service reset is in progress.

|   |   |
|:---|:---|
|Message Format|"A reset on %1 is in progress."
|Severity|Warning
|Resolution|Wait for device or service reset to complete, and then retry the operation.

### HpeCommon.ResetRequired

**Description:**  One or more properties were changed, but these changes will not take effect until the device or service is reset.

|   |   |
|:---|:---|
|Message Format|"One or more properties were changed, but these changes will not take effect until %1 is reset."
|Severity|Warning
|Resolution|To enable the changed properties, reset the device or service.

### HpeCommon.ResourceNotReadyRetry

**Description:**  The resource is present but is not ready to perform operations due to an internal condition such as initialization or reset.

|   |   |
|:---|:---|
|Message Format|"The resource is present but is not ready to perform operations.  The resource will be ready in %1 seconds."
|Severity|Warning
|Resolution|Retry the operation when the resource is ready.

### HpeCommon.SuccessFeedback

**Description:**  The operation completed successfully

|   |   |
|:---|:---|
|Message Format|"The operation completed successfully"
|Severity|OK
|Resolution|None

### HpeCommon.TaskCreated

**Description:**  A task was created in response to the operation.

|   |   |
|:---|:---|
|Message Format|"A task was created in response to the operation and is accessible at %1."
|Severity|OK
|Resolution|Perform an HTTP GET request on the supplied URI for task status.

### HpeCommon.UnsupportedHwConfiguration

**Description:**  A previously requested property value change was reverted because the current hardware configuration does not support it.

|   |   |
|:---|:---|
|Message Format|"The value %1 for property %2 was reverted because the current hardware configuration does not support it."
|Severity|Warning
|Resolution|Ensure that the system's hardware configuration supports the property value.

### iLO.AHSDisabled

**Description:**  Modifying AHS properties is not possible with AHS disabled.

|   |   |
|:---|:---|
|Message Format|"Modifying AHS properties is not possible with AHS disabled."
|Severity|Warning
|Resolution|Enable AHS, and then modify the AHS properties.

### iLO.Accepted

**Description:**  Indicates that one or more properties were correctly changed, but may not be in effect yet.

|   |   |
|:---|:---|
|Message Format|"Indicates that one or more properties were correctly changed, but may not be in effect yet."
|Severity|OK
|Resolution|None

### iLO.ActionParameterValueNotInList

**Description:**  Indicates that the correct value type was supplied for the action parameter, but the value is not supported. (The value is not in the enumeration list.)

|   |   |
|:---|:---|
|Message Format|"The value %1 for the property %2 is not in the list of valid values."
|Severity|Warning
|Resolution|Choose a value from the enumeration list and resubmit the request if the operation failed.

### iLO.AlertMailFeatureDisabled

**Description:**  AlertMail feature is disabled.

|   |   |
|:---|:---|
|Message Format|"AlertMail feature is disabled."
|Severity|Warning
|Resolution|Enable AlertMail feature to send test alert message.

### iLO.AlreadyInProgress

**Description:**  An operation is already in progress.

|   |   |
|:---|:---|
|Message Format|"An operation is already in progress."
|Severity|Warning
|Resolution|Wait for the current operation to complete, and then retry the operation.

### iLO.AlreadyUpToDate

**Description:**  

|   |   |
|:---|:---|
|Message Format|"The update did not occur because the component was already up to date."
|Severity|Warning
|Resolution|None.

### iLO.ArrayPropertyOutOfBound

**Description:**  The number of items in the array exceeds the maximum number supported.

|   |   |
|:---|:---|
|Message Format|"An array %1 was supplied with %2 items that exceeds the maximum supported count of %3."
|Severity|Warning
|Resolution|Retry the operation using the correct number of items for the array.

### iLO.BiosActionTBD

**Description:**  The BIOS action supplied in the POST operation is not yet implemented.

|   |   |
|:---|:---|
|Message Format|"The BIOS action %1 is not implemented yet."
|Severity|Critical
|Resolution|The action was invalid or the wrong resource was the target. See the implementation documentation for assistance.

### iLO.BiosPasswordInfoInvalid

**Description:**  The stored BIOS password information is invalid. A system reboot is neccessary to retore password defaults.

|   |   |
|:---|:---|
|Message Format|"The stored BIOS password information is invalid.  Reboot system."
|Severity|Critical
|Resolution|The system will need to be rebooted to restore BIOS password information to defaults.

### iLO.BiosPasswordMismatch

**Description:**  The provided OldPassword does not match the stored BIOS password.

|   |   |
|:---|:---|
|Message Format|"The provided OldPassword does not match the stored BIOS password."
|Severity|Critical
|Resolution|Retry the action with the matching password.

### iLO.CannotRemoveLicense

**Description:**  Cannot remove iLO Standard/iLO Standard for BladeSystem license.

|   |   |
|:---|:---|
|Message Format|"Cannot remove iLO Standard/iLO Standard for BladeSystem license."
|Severity|Warning
|Resolution|None.

### iLO.ComponentUploadAlreadyInProgress

**Description:**  A component upload operation is already in progress.

|   |   |
|:---|:---|
|Message Format|"A component upload operation is already in progress."
|Severity|Warning
|Resolution|Wait for the current component upload to complete, and then retry the operation.

### iLO.ComponentUploadFailed

**Description:**  A component upload operation failed.

|   |   |
|:---|:---|
|Message Format|"A component upload operation failed."
|Severity|Warning
|Resolution|Wait for the current component upload to complete, and then retry the operation.

### iLO.DemoLicenseKeyPreviouslyInstalled

**Description:**  A demo license was previously installed.

|   |   |
|:---|:---|
|Message Format|"A demo license was previously installed."
|Severity|Warning
|Resolution|None.

### iLO.DeviceResetRequired

**Description:**  Indicates that one or more properties were correctly changed, but will not take effect until device is reset.

|   |   |
|:---|:---|
|Message Format|"One or more properties were changed and will not take effect until the device is reset."
|Severity|Warning
|Resolution|Reset the device for the settings to take effect.

### iLO.DiagsTestAlreadyRunning

**Description:**  A diagnostics self test is already running.

|   |   |
|:---|:---|
|Message Format|"A diagnostics self test is already running."
|Severity|Warning
|Resolution|Stop the running test and try again.

### iLO.ESKMServersNotConfigured

**Description:**  Enterprise Secure Key Manager Servers are not configured.

|   |   |
|:---|:---|
|Message Format|"Enterprise Secure Key Manager Servers are not configured."
|Severity|OK
|Resolution|None.

### iLO.ETagTooLong

**Description:**  The supplied ETag is too long. The maximum supported ETag length is 63 bytes.

|   |   |
|:---|:---|
|Message Format|"The supplied ETag is too long. The maximum supported ETag length is 63 bytes."
|Severity|Warning
|Resolution|Retry the operation using an ETag with a length of 63 bytes or less.

### iLO.EmptyDNSName

**Description:**  DNS name is empty.

|   |   |
|:---|:---|
|Message Format|"Empty DNS name."
|Severity|Warning
|Resolution|Retry the request with a valid DNS name.

### iLO.ErrorIntializingESKM

**Description:**  Failed to initialize ESKM.

|   |   |
|:---|:---|
|Message Format|"Failed to initialize ESKM."
|Severity|Warning
|Resolution|Check if Account Group, Local CA Certificate Name, Login Name and Password are correct and try again.

### iLO.EventLogCleared

**Description:**  Event log cleared successfully.

|   |   |
|:---|:---|
|Message Format|"Event log cleared successfully."
|Severity|OK
|Resolution|None.

### iLO.EventSubscriptionModified

**Description:**  The event subscription was modified successfully.

|   |   |
|:---|:---|
|Message Format|"The event subscription was modified successfully."
|Severity|OK
|Resolution|None.

### iLO.EventSubscriptionRemoved

**Description:**  The event subscription was removed successfully.

|   |   |
|:---|:---|
|Message Format|"The event subscription was removed successfully."
|Severity|OK
|Resolution|None.

### iLO.ExtendedInfo

**Description:**  Indicates that extended information is available.

|   |   |
|:---|:---|
|Message Format|"See @Message.ExtendedInfo for more information."
|Severity|OK
|Resolution|See @Message.ExtendedInfo for more information.

### iLO.FWFlashSuccessTPMOverrideEnabled

**Description:**  A Trusted Module is  detected in this system. If you have not performed the proper OS encryption procedures, you will lose access to your data if recovery key is not available. Recommended procedure is to suspend encryption software prior to System ROM or Option ROM firmware flash. TPMOverrideFlag is enabled and firmware flash initiated.

|   |   |
|:---|:---|
|Message Format|"CAUTION: A Trusted Module is detected in this system. Updating the System ROM or Option Card Firmware may have impact to measurements stored in the TM and may have impact to security functionality on the platform which depends on these measurements."
|Severity|OK
|Resolution|None.

### iLO.FWFlashSuccessTrustedModuleOverrideEnabled

**Description:**  A Trusted Module (type unspecified) is installed in the system and TPMOverrideFlag is enabled. Firmware flash initiated.

|   |   |
|:---|:---|
|Message Format|"CAUTION: A Trusted Module (type unspecified) has been detected in this system. If you have not performed the proper OS encryption procedures, you will lose access to your data if recovery key is not available. Recommended procedure for Microsoft Windows(R) BitLocker(TM) is to "suspend" BitLocker prior to System ROM or Option ROM firmware flash."
|Severity|OK
|Resolution|None.

### iLO.FWFlashTPMOverrideFlagRequired

**Description:**  A Trusted Module is  detected in this system. Failure to perform proper OS encryption procedures will result in loss of access to your data if recovery key is not available. Recommended procedure is to suspend encryption software prior to System ROM or Option ROM firmware flash. If you do not have your recovery key or have not suspended encryption software, cancel this firmware upload. Failure to follow these instructions will result in loss of access to your data. To continue with firmware flash TPMOverrideFlag is required.

|   |   |
|:---|:---|
|Message Format|"CAUTION: A Trusted Module is detected in this system. Updating the System ROM or Option Card Firmware may have impact to measurements stored in the TM and may have impact to security functionality on the platform which depends on these measurements."
|Severity|Warning
|Resolution|Please set the TPMOverrideFlag to true and try again.

### iLO.FWFlashTrustedModuleOverrideFlagRequired

**Description:**  A Trusted Module (type unspecified) is installed in the system, TPMOverrideFlag is required for firmware flash to proceed.

|   |   |
|:---|:---|
|Message Format|"CAUTION: A Trusted Module (type unspecified) has been detected in this system. Failure to perform proper OS encryption procedures will result in loss of access to your data if recovery key is not available. Recommended procedure for Microsoft Windows(R) BitLocker(TM) is to "suspend" BitLocker prior to System ROM or Option ROM firmware flash. If you do not have your recovery key or have not suspended BitLocker, exit this flash: Failure to follow these instructions will result in loss of access to your data."
|Severity|Warning
|Resolution|Please set the TPMOverrideFlag to true and try again.

### iLO.FirmwareFlashAlreadyInProgress

**Description:**  A firmware upgrade operation is already in progress.

|   |   |
|:---|:---|
|Message Format|"A firmware flash operation is already in progress."
|Severity|Warning
|Resolution|Wait for the current firmware flash to complete, and then retry the operation.

### iLO.GeneratingCertificate

**Description:**  Generating the X509 Certificate.

|   |   |
|:---|:---|
|Message Format|"X509 Certificate is being generated and the process might take up to 10 minutes."
|Severity|OK
|Resolution|None.

### iLO.ICRUInvalidAddress

**Description:**  ICRU returned invalid address for translation.

|   |   |
|:---|:---|
|Message Format|"ICRU returned invalid address for translation."
|Severity|Warning
|Resolution|Input valid address for translation.

### iLO.ICRUNotSupported

**Description:**  ICRU feature or function is not supported on the system.

|   |   |
|:---|:---|
|Message Format|"ICRU feature or function is not supported on the system."
|Severity|Warning
|Resolution|None.

### iLO.IPv6ConfigurationError

**Description:**  The specified IPv6 configuration caused an error.

|   |   |
|:---|:---|
|Message Format|"The specified IPv6 configuration was in error due to %1."
|Severity|Warning
|Resolution|Resolve the indicated error in the configuration data.

### iLO.ImportCertSuccessful

**Description:**  Import Certificate was successful.

|   |   |
|:---|:---|
|Message Format|"Import Certificate was successful."
|Severity|OK
|Resolution|None.

### iLO.ImportCertSuccessfuliLOResetinProgress

**Description:**  Import Certificate was successful and the management processor is being reset.

|   |   |
|:---|:---|
|Message Format|"Import Certificate was successful. Management Processor reset is in progress to enable the new certificate."
|Severity|Warning
|Resolution|None.

### iLO.ImportCertificateFailed

**Description:**  Failed importing Certificate.

|   |   |
|:---|:---|
|Message Format|"Failed importing the X509 Certificate."
|Severity|Warning
|Resolution|Retry the operation with proper Certificate information.

### iLO.ImportSSOParamError

**Description:**  Not a valid parameter.

|   |   |
|:---|:---|
|Message Format|"Invalid Parameter."
|Severity|Warning
|Resolution|Retry the request with valid parameters.

### iLO.ImportSSOUriError

**Description:**  Not a valid Uri to import SSO certificate.

|   |   |
|:---|:---|
|Message Format|"Invalid Uri."
|Severity|Warning
|Resolution|Retry the request with valid URI.

### iLO.IndicatorLedInvalidStateChange

**Description:**  The request to change the state of the Indicator LED cannot be granted because the current state is either Blinking or is Unknown.

|   |   |
|:---|:---|
|Message Format|"The Indicator LED cannot be changed when its state is Blinking or Unknown."
|Severity|Warning
|Resolution|Please wait until the server has completed its reserved state.

### iLO.InstallSetWriteError

**Description:**  The InstallSet write failed.

|   |   |
|:---|:---|
|Message Format|"The InstallSet write of %1 failed."
|Severity|Warning
|Resolution|Ensure a valid name for the item and that space exists to hold the item.

### iLO.InterfaceDisabledResetRequired

**Description:**  Disabling one or more interfaces/features will cause certain functionalities to be not available. Please refer to User Guide for details on the implications. Changes will not take effect until the management processor is reset

|   |   |
|:---|:---|
|Message Format|"CAUTION: Disabling one or more interfaces/features will cause certain functionalities to be not available. Please refer to User Guide for details on the implications. Changes will not take effect until the management processor is reset"
|Severity|OK
|Resolution|None.

### iLO.InternalErrorWithParam

**Description:**  The operation was not successful due to an internal service error (shown), but the service is still operational.

|   |   |
|:---|:---|
|Message Format|"The operation was not successful due to an internal service error (%1), but the service is still operational."
|Severity|Critical
|Resolution|Retry the operation. If the problem persists, consider resetting the service.

### iLO.InvalidConfigurationSpecified

**Description:**  The specified configuration is not valid.

|   |   |
|:---|:---|
|Message Format|"The specified configuration is not valid."
|Severity|Warning
|Resolution|Correct the configuration, and then retry the operation.

### iLO.InvalidConfigurationSpecifiedForFederation

**Description:**  iLO Federation Management cannot be supported in the current configuration.

|   |   |
|:---|:---|
|Message Format|"iLO Federation Management cannot be supported in the current configuration."
|Severity|Warning
|Resolution|Review the management processor network settings or Onboard Administrator settings and refer to the User Guide.

### iLO.InvalidEngineID

**Description:**  EngineID should be a hexadecimal number starting with 0x (for example, 0x0102030405abcdef). The string length should be an even number, greater than or equal to 6 characters (excluding the "0x"), and less than or equal to 32 characters.

|   |   |
|:---|:---|
|Message Format|"EngineID should be a hexadecimal number starting with 0x (for example, 0x0102030405abcdef). The string length should be an even number, greater than or equal to 6 characters (excluding the "0x"), and less than or equal to 32 characters."
|Severity|Warning
|Resolution|Retry the operation using an EngineID within the specified parameters.

### iLO.InvalidIndex

**Description:**  The Index is not valid.

|   |   |
|:---|:---|
|Message Format|"The Index provided is not valid."
|Severity|Warning
|Resolution|Adhere to the indexes supported in the self links.

### iLO.InvalidLicenseKey

**Description:**  The license key is not valid.

|   |   |
|:---|:---|
|Message Format|"The license key is not valid."
|Severity|Warning
|Resolution|Retry the operation using a valid license key.

### iLO.InvalidOperationForAutoPowerOnState

**Description:**  The operation was not successful because the current auto power on mode specifies power is to remain off.

|   |   |
|:---|:---|
|Message Format|"The auto power on delay cannot be set because power is configured to remain off."
|Severity|Warning
|Resolution|Verify that the system auto power on mode is set to turn power on or follow the previous power setting.

### iLO.InvalidOperationForSystemState

**Description:**  The operation was not successful due to the current power state (for example, attempting to turn the power off when it is already off).

|   |   |
|:---|:---|
|Message Format|"The operation was not successful due to the current power state."
|Severity|Warning
|Resolution|Verify that the system is in the correct power state, and then retry the operation.

### iLO.InvalidPassphraseLength

**Description:**  The passphrase must contain 8 to 49 characters.

|   |   |
|:---|:---|
|Message Format|"%1 must contain 8 to 49 characters."
|Severity|Warning
|Resolution|Correct the passphrase, and then retry the operation.

### iLO.InvalidPasswordLength

**Description:**  The password length is not valid.

|   |   |
|:---|:---|
|Message Format|"A valid password must contain between %1 to %2 characters."
|Severity|Critical
|Resolution|Retry the operation using a corrected password.

### iLO.LicenseKeyNotSupported

**Description:**  The use of a license key is not supported on this system.

|   |   |
|:---|:---|
|Message Format|"The use of a license key is not supported on this system."
|Severity|Warning
|Resolution|None.

### iLO.LicenseKeyRequired

**Description:**  A license key is required to use this operation or feature.

|   |   |
|:---|:---|
|Message Format|"A license key is required to use this operation or feature."
|Severity|Warning
|Resolution|Install a license key to use this feature.

### iLO.LoginAttemptDelayed

**Description:**  The login was not successful, so the service enforces a delay before another login is allowed.

|   |   |
|:---|:---|
|Message Format|"The login was not successful, so the service enforces a delay before another login is allowed."
|Severity|Warning
|Resolution|Wait for the delay time to expire, and then retry the login.

### iLO.LoginAttemptDelayedSeconds

**Description:**  The login was not successful, so the service enforces a delay before another login is allowed.

|   |   |
|:---|:---|
|Message Format|"The login was not successful, so the service enforces a %1 second delay before another login is allowed."
|Severity|Warning
|Resolution|None.

### iLO.MaxProviders

**Description:**  The maximum number of providers are already registered.

|   |   |
|:---|:---|
|Message Format|"The maximum number of providers are already registered."
|Severity|Warning
|Resolution|None.

### iLO.MaxVirtualMediaConnectionEstablished

**Description:**  No more Virtual Media connections are available, because the maximum number of connections are already established.

|   |   |
|:---|:---|
|Message Format|"No more Virtual Media connections are available, because the maximum number of connections are already established."
|Severity|Warning
|Resolution|Close an established Virtual Media connection, and then retry creating or opening another connection.

### iLO.MembistVariablesNotSupported

**Description:**  Membist variables are not supported on the system.

|   |   |
|:---|:---|
|Message Format|"Membist variables are not supported on the system."
|Severity|Warning
|Resolution|None.

### iLO.NoEventSubscriptions

**Description:**  There are no event subscriptions registerd.

|   |   |
|:---|:---|
|Message Format|"The opeartion can not be completed because there are no event subscribers."
|Severity|Warning
|Resolution|

### iLO.NoPowerMetering

**Description:**  No support for power metering available on platform.

|   |   |
|:---|:---|
|Message Format|"No support for power metering available on platform."
|Severity|OK
|Resolution|Enable Power Metering on platform if supported.

### iLO.NoSNMPAlertDestinationsConfigured

**Description:**  No SNMP alert destinations are configured.

|   |   |
|:---|:---|
|Message Format|"No SNMP alert destinations are configured."
|Severity|Warning
|Resolution|Disable SNMP pass-thru, modify the property, and then re-enable SNMP pass-thru.

### iLO.NoSamples

**Description:**  No power history samples are available.

|   |   |
|:---|:---|
|Message Format|"No power history samples are available."
|Severity|OK
|Resolution|To accumulate power history samples, power on the server, and then wait at least 5 minutes.

### iLO.NoScriptedVirtualMediaConnectionAvailable

**Description:**  No scripted virtual media connections exist to perform the operation.

|   |   |
|:---|:---|
|Message Format|"No scripted virtual media connections exist to perform the operation."
|Severity|Warning
|Resolution|Create or open a scripted virtual media connection, and then retry the operation.

### iLO.NoSpaceforDNSName

**Description:**  No space to store DNS name.

|   |   |
|:---|:---|
|Message Format|"No space to store DNS name."
|Severity|Warning
|Resolution|Make sure SSO database has enough space to store DNS name.

### iLO.NoVirtualMediaConnectionAvailable

**Description:**  No Virtual Media connections exist to perform the operation.

|   |   |
|:---|:---|
|Message Format|"No Virtual Media connections exist to perform the operation."
|Severity|Warning
|Resolution|Create or open a Virtual Media connection, and then retry the operation.

### iLO.NotSupportedOnNIC

**Description:**  This property is not supported by the indicated network port.

|   |   |
|:---|:---|
|Message Format|"%1 is not supported on the %2 Network Port."
|Severity|Warning
|Resolution|Do not specify this property on the indicated network port.

### iLO.NotValidIPAddrOrDNS

**Description:**  The value for the property is not a valid IPv4/v6 address or DNS name.

|   |   |
|:---|:---|
|Message Format|"The value for property %1 is not a valid IPv4/v6 address or DNS name."
|Severity|Warning
|Resolution|Correct the IPv4/v6 address or DNS name, and then retry the operation.

### iLO.NotValidIPAddress

**Description:**  The value for the property is not a valid IP address.

|   |   |
|:---|:---|
|Message Format|"The value %1 is not a valid IP address for %2"
|Severity|Warning
|Resolution|Use a valid IP address.

### iLO.NotValidSubnetMask

**Description:**  The value for the property is not a valid subnet mask.

|   |   |
|:---|:---|
|Message Format|"The value %1 is not a valid subnet mask for %2"
|Severity|Warning
|Resolution|Use a valid subnet mask.

### iLO.OperationWillCompleteAfterSystemPOST

**Description:**  The value for the property will be applied after System BIOS POST completes.

|   |   |
|:---|:---|
|Message Format|"The value for property %1 will be changed after the System BIOS completes POST."
|Severity|Information
|Resolution|Wait to see the change in value until after the System BIOS completes POST.

### iLO.PowerCapOACntrld

**Description:**  The enclosure Onboard Administrator is currently managing the power cap.

|   |   |
|:---|:---|
|Message Format|"The enclosure Onboard Administrator is currently managing the power cap."
|Severity|Warning
|Resolution|Use Onboard Administrator to Manage the PowerCap

### iLO.PowerCapROMCntrld

**Description:**  The System ROM is currently managing the power cap.

|   |   |
|:---|:---|
|Message Format|"The System ROM is currently managing the power cap."
|Severity|Warning
|Resolution|Enable RESTful API management of the power cap in System ROM

### iLO.PowerValueBadParam

**Description:**  The power cap value is not valid.

|   |   |
|:---|:---|
|Message Format|"The power cap value is not valid."
|Severity|Warning
|Resolution|Retry the operation using a corrected value.

### iLO.PowerValueInvalidCalibrationData

**Description:**  The request to set the power cap failed. Invalid power cap calibration data. The Power Cap feature is currently unavailable.

|   |   |
|:---|:---|
|Message Format|"The request to set the power cap failed. Invalid power cap calibration data. The Power Cap feature is currently unavailable"
|Severity|Warning
|Resolution|Restart the server to retrieve calibration data from initial POST.

### iLO.PowerValueNotOptimal

**Description:**  Power caps set for less than 50% of the difference between maximum and minimum power may become unreachable due to changes in the server. Power caps set for less than 20% are not recommended.

|   |   |
|:---|:---|
|Message Format|"Power caps set for less than 50% of the difference between maximum and minimum power may become unreachable due to changes in the server. Power caps set for less than 20% are not recommended."
|Severity|Warning
|Resolution|Please provide an optimal value in integer considering the power cap range.

### iLO.PowerValueUnAvailable

**Description:**  Advanced power capping is not currently available due to the system configuration or state.

|   |   |
|:---|:---|
|Message Format|"Advanced power capping is not currently available due to the system configuration or state."
|Severity|Warning
|Resolution|Change the system configuration or wait for the system to become fully initialized, and then retry the operation.

### iLO.PowerValueUnSupported

**Description:**  Advanced power capping is not supported on this system.

|   |   |
|:---|:---|
|Message Format|"Advanced power capping is not supported on this system."
|Severity|Warning
|Resolution|None.

### iLO.PrimaryESKMServerAccessible

**Description:**  Only the primary ESKM server is accessible.

|   |   |
|:---|:---|
|Message Format|"No redundancy. Only the primary ESKM server is accessible."
|Severity|OK
|Resolution|None.

### iLO.PrimarySecondaryAddressesResolveToSameServer

**Description:**  Primary and secondary ESKM server addresses resolve to the same server.

|   |   |
|:---|:---|
|Message Format|"No redundancy. Primary and secondary ESKM server addresses resolve to the same server."
|Severity|OK
|Resolution|None.

### iLO.PrimarySecondaryESKMServersAccessible

**Description:**  Both primary and secondary ESKM servers are accessible.

|   |   |
|:---|:---|
|Message Format|"Redundant solution: Both primary and secondary ESKM servers are accessible."
|Severity|OK
|Resolution|None.

### iLO.PropertyNotWritableOrUnknown

**Description:**  The request included a value for a  read-only or unknown property.

|   |   |
|:---|:---|
|Message Format|"The property %1 is a read-only property and cannot be assigned a value, or not valid for this resource."
|Severity|Warning
|Resolution|If the operation did not complete, remove the property from the request body and resubmit the request.

### iLO.PropertyValueBadParam

**Description:**  The property value is not valid.

|   |   |
|:---|:---|
|Message Format|"The property value is not valid."
|Severity|Warning
|Resolution|Retry the operation using a corrected value.

### iLO.PropertyValueExceedsMaxLength

**Description:**  The value for the property exceeds the maximum length.

|   |   |
|:---|:---|
|Message Format|"The value %1 for the property %2 exceeds the maximum length of %3."
|Severity|Warning
|Resolution|Correct the value for the property in the request body, and then retry the operation.

### iLO.PropertyValueIncompatible

**Description:**  The value for the property is the correct type, but this value is incompatible with the current value of another property.

|   |   |
|:---|:---|
|Message Format|"The value %1 for the property %2 is incompatible with the value for property %3."
|Severity|Warning
|Resolution|Correct the value for the property in the request body, and then retry the operation.

### iLO.PropertyValueOutOfRange

**Description:**  The value for the property is out of range.

|   |   |
|:---|:---|
|Message Format|"The value %1 for the property %2 is out of range %3."
|Severity|Warning
|Resolution|Correct the value for the property in the request body, and then retry the operation.

### iLO.PropertyValueRequired

**Description:**  Indicates that a property was required but not specified.

|   |   |
|:---|:---|
|Message Format|"%1 requires Property %2 to be specified."
|Severity|Warning
|Resolution|Include the required property in the request body and then retry the operation.

### iLO.RepairNotSupported

**Description:**  IML event with this severity is not supported to be repaired. IML events with Critical or Warning severities can marked as repaired.

|   |   |
|:---|:---|
|Message Format|"IML event with %1 severity is not supported to be repaired. IML events with Critical or Warning severities can marked as repaired."
|Severity|Warning
|Resolution|Please do not try to repair IML events with severity other than Critical or Warning.

### iLO.RequiredPropertyMissing

**Description:**  Indicates that a required property is not specified.

|   |   |
|:---|:---|
|Message Format|"Required Property %1 needs to be specifed."
|Severity|Warning
|Resolution|Include the required property in the request body and then retry the operation.

### iLO.ResetInProgress

**Description:**  A management processor reset is in progress.

|   |   |
|:---|:---|
|Message Format|"A management processor reset is in progress."
|Severity|Warning
|Resolution|Wait for management processor reset to complete, and then retry the operation.

### iLO.ResetRequired

**Description:**  One or more properties were changed, but these changes will not take effect until the management processor is reset.

|   |   |
|:---|:---|
|Message Format|"One or more properties were changed, but these changes will not take effect until the management processor is reset."
|Severity|Warning
|Resolution|To enable the changed properties, reset the management processor.

### iLO.ResourceBeingFlashed

**Description:**  The change to the requested resource failed because the resource is being flashed.

|   |   |
|:---|:---|
|Message Format|"The change to the requested resource failed because the resource is being flashed."
|Severity|Warning
|Resolution|Retry the operation when the firmware upgrade has completed.

### iLO.ResourceInUseWithDetail

**Description:**  The change could not be made because the resource was in use or in a transitioning state.

|   |   |
|:---|:---|
|Message Format|"The change to the resource failed because the resource is in use or in transition."
|Severity|Warning
|Resolution|Retry the request.

### iLO.ResourceTemporarilyUnavailable

**Description:**  The resource is temporarily unavailable because the firmware is being flashed.

|   |   |
|:---|:---|
|Message Format|"The resource is temporarily unavailable because the firmware is being flashed."
|Severity|Warning
|Resolution|Retry the operation when the firmware upgrade has completed.

### iLO.SMBIOSRecordNotFound

**Description:**  The SMBIOS record type is not found or is not supported on the system.

|   |   |
|:---|:---|
|Message Format|"The SMBIOS record type %1 is not found or is not supported on the system."
|Severity|Warning
|Resolution|Reset the system to update the SMBIOS records. If the problem persists then the SMBIOS record type is not supported.

### iLO.SNMPAlertDisabled

**Description:**  The operation could not be completed because SNMP alerts are disabled.

|   |   |
|:---|:---|
|Message Format|"The operation could not be completed because SNMP alerts are disabled."
|Severity|Warning
|Resolution|Enable SNMP alerts and retry the operation.

### iLO.SNMPDisabled

**Description:**  Modifying SNMP properties is not possible with SNMP disabled.

|   |   |
|:---|:---|
|Message Format|"Modifying SNMP properties is not possible with SNMP disabled."
|Severity|Warning
|Resolution|Enable SNMP, and then modify the SNMP properties.

### iLO.SNMPTestAlertFailed

**Description:**  The SNMP Test Alert did not send successfully.

|   |   |
|:---|:---|
|Message Format|"The SNMP Test Alert did not send successfully."
|Severity|Warning
|Resolution|Verify the test alert content and retry.

### iLO.SNTPConfigurationManagedByDHCPAndIsReadOnly

**Description:**  SNTP configuration is currently managed by DHCP and is therefore read-only.

|   |   |
|:---|:---|
|Message Format|"%1 cannot be changed while DHCP is configured to provide SNTP settings."
|Severity|Warning
|Resolution|Disable SNTP configuration options in both DHCPv4 and DHCPv6 (see /Managers/n/NICs), and then reconfigure SNTP as desired with static settings.

### iLO.SSOCertficateEmpty

**Description:**  SSO Certificate is Empty.

|   |   |
|:---|:---|
|Message Format|"Empty SSO Certificate."
|Severity|Warning
|Resolution|None.

### iLO.SSOCertificateReadError

**Description:**  SSO Certificate Read Error.

|   |   |
|:---|:---|
|Message Format|"Error reading SSO certificate."
|Severity|Warning
|Resolution|Retry the request with valid SSO certificate.

### iLO.SSONoSpaceError

**Description:**  No space to store SSO certificate.

|   |   |
|:---|:---|
|Message Format|"No space to store SSO certificate."
|Severity|Warning
|Resolution|Make sure SSO database has enough space to store SSO certificate.

### iLO.SSORecordNotFound

**Description:**  SSO Record Not Found.

|   |   |
|:---|:---|
|Message Format|"SSO Record Not Found."
|Severity|Warning
|Resolution|None.

### iLO.SecondaryESKMServerAccessible

**Description:**  Only the secondary ESKM server is accessible.

|   |   |
|:---|:---|
|Message Format|"No redundancy. Only the secondary ESKM server is accessible."
|Severity|OK
|Resolution|None.

### iLO.SuccessFeedback

**Description:**  The operation completed successfully.

|   |   |
|:---|:---|
|Message Format|"The operation completed successfully."
|Severity|OK
|Resolution|None

### iLO.SyslogFeatureDisabled

**Description:**  Remote Syslog feature is disabled.

|   |   |
|:---|:---|
|Message Format|"Remote syslog feature is disabled."
|Severity|Warning
|Resolution|Enable remote syslog feature to send test syslog message.

### iLO.SystemResetRequired

**Description:**  The system properties were correctly changed, but will not take effect until the system is reset.

|   |   |
|:---|:---|
|Message Format|"One or more properties were changed and will not take effect until system is reset."
|Severity|Warning
|Resolution|Reset system for the settings to take effect.

### iLO.TokenRequired

**Description:**  Proper 'X-HPRESTFULAPI-AuthToken' authorization token not provided.

|   |   |
|:---|:---|
|Message Format|"Proper 'X-HPRESTFULAPI-AuthToken' authorization token not provided."
|Severity|Critical
|Resolution|Create proper 'X-HPRESTFULAPI-AuthToken' authorization token. Send token in using the proper HTTP header.

### iLO.UnableModifyRights

**Description:**  Unable to modify user rights.

|   |   |
|:---|:---|
|Message Format|"Unable to modify user rights."
|Severity|Warning
|Resolution|None.

### iLO.UnableToModifyDueToMissingComponent

**Description:**  The value for the property cannot be changed because a related hardware component is not installed.

|   |   |
|:---|:---|
|Message Format|"The value for property %1 cannot be changed because a related hardware component is not installed."
|Severity|Warning
|Resolution|Install the hardware component and retry the operation.

### iLO.UnableToModifyDuringSystemPOST

**Description:**  The value for the property cannot be changed while the computer system BIOS is in POST.

|   |   |
|:---|:---|
|Message Format|"The value for property %1 cannot be changed while the computer system BIOS is in POST."
|Severity|Warning
|Resolution|After the computer system is either fully booted or powered off, retry the operation.

### iLO.UnauthorizedLoginAttempt

**Description:**  The login was not successful, because the supplied credentials could not be authorized.

|   |   |
|:---|:---|
|Message Format|"The login was not successful, because the supplied credentials could not be authorized."
|Severity|Warning
|Resolution|Log in with authorized user name and password credentials.

### iLO.UnsupportedOperation

**Description:**  This operation is not supported by RIS for the current system.

|   |   |
|:---|:---|
|Message Format|"This operation is not supported by RIS for the current system."
|Severity|Warning
|Resolution|None.

### iLO.UnsupportedOperationInLegacyBootMode

**Description:**  This operation is not supported when the system Boot Mode is set to Legacy BIOS.

|   |   |
|:---|:---|
|Message Format|" This operation is not supported when the system Boot Mode is set to Legacy BIOS."
|Severity|Warning
|Resolution|Change the Boot Mode to UEFI and retry the operation.

### iLO.UnsupportedOperationInSystemBIOS

**Description:**  This operation is not supported by the current version of the system BIOS.

|   |   |
|:---|:---|
|Message Format|"This operation is not supported by the current version of the system BIOS."
|Severity|Warning
|Resolution|None.

### iLO.UpdateBadParameter

**Description:**  

|   |   |
|:---|:---|
|Message Format|"The update failed because a bad parameter was supplied."
|Severity|Warning
|Resolution|Supply correct parameters to the component and retry the update.

### iLO.UpdateCancelled

**Description:**  

|   |   |
|:---|:---|
|Message Format|"The update was canceled by the update process."
|Severity|Warning
|Resolution|Retry the update.

### iLO.UpdateDependencyFailure

**Description:**  

|   |   |
|:---|:---|
|Message Format|"The update did not complete because the component failed a dependency check."
|Severity|Warning
|Resolution|Install any dependent components first and then retry this update.

### iLO.UpdateFailed

**Description:**  

|   |   |
|:---|:---|
|Message Format|"The update failed with a component specific error (%1)."
|Severity|Warning
|Resolution|Retry the update after remedying the component error.

### iLO.UpdateInPOST

**Description:**  

|   |   |
|:---|:---|
|Message Format|"System must not be booted past POST in order to perform this update"
|Severity|Warning
|Resolution|Boot to UEFI and retry the update.

### iLO.UpdateInterrupted

**Description:**  

|   |   |
|:---|:---|
|Message Format|"The update was interrupted."
|Severity|Warning
|Resolution|Retry the update.

### iLO.UpdateInvalidFile

**Description:**  

|   |   |
|:---|:---|
|Message Format|"The update operation failed because the file is not valid."
|Severity|Warning
|Resolution|Remove and re-add the component to the repository and try the operation again.

### iLO.UpdateInvalidOS

**Description:**  

|   |   |
|:---|:---|
|Message Format|"The update did not occur because the running OS is not valid."
|Severity|Warning
|Resolution|Retry the update while running the correct OS.

### iLO.UpdateNotApplicable

**Description:**  

|   |   |
|:---|:---|
|Message Format|"The task was not completed because the component was not applicable to this system."
|Severity|Warning
|Resolution|None.

### iLO.UpdateRepositoryUnavailable

**Description:**  

|   |   |
|:---|:---|
|Message Format|"The update operation failed because the component repository is unavailable."
|Severity|Warning
|Resolution|None.

### iLO.UpdateTaskQueueFull

**Description:**  The Invoke action was not successful because the update task queue is full.

|   |   |
|:---|:---|
|Message Format|"The Invoke action was not successful because the update task queue is full."
|Severity|Critical
|Resolution|Remove completed tasks from the update task queue to retry the operation.

### iLO.UpdateTaskQueueWriteError

**Description:**  The UpdateTaskQueue write failed.

|   |   |
|:---|:---|
|Message Format|"The UpdateTaskQueue write of %1 failed."
|Severity|Warning
|Resolution|Ensure a valid name for the item and that space exists to hold the item.

### iLO.UpdateTemporarilyUnavailable

**Description:**  

|   |   |
|:---|:---|
|Message Format|"The system is temporarily unable to perform this update"
|Severity|Warning
|Resolution|Retry the update, ensuring that power state is stable.

### iLO.UpdateWithPowerOff

**Description:**  

|   |   |
|:---|:---|
|Message Format|"System power must be off to perform this update"
|Severity|Warning
|Resolution|Power system on and retry the update.

### iLO.UpdateWithPowerOn

**Description:**  

|   |   |
|:---|:---|
|Message Format|"System power must be on to perform this update"
|Severity|Warning
|Resolution|Power system on and retry the update.

### iLO.UserAlreadyExist

**Description:**  The user or login user name already exists.

|   |   |
|:---|:---|
|Message Format|"The user or login user name already exists."
|Severity|Warning
|Resolution|Try a different user or login user name.

### iLO.UserNameAlreadyExists

**Description:**  Duplicate SNMPv3 User.

|   |   |
|:---|:---|
|Message Format|"The username %1 already exists in the list"
|Severity|Warning
|Resolution|Enter a different name and try again.

### iLO.VirtualMediaIsDisabled

**Description:**  Virtual Media has been disabled.

|   |   |
|:---|:---|
|Message Format|"Virtual Media has been disabled."
|Severity|Warning
|Resolution|Enable Virtual Media to perform this operation.

### iLO.iLOResetAndSystemRebootRequired

**Description:**  Indicates that one or more properties were correctly changed, but will not take effect until device is reset and system is rebooted.

|   |   |
|:---|:---|
|Message Format|"One or more properties were changed and will not take effect until the device is reset and system is rebooted"
|Severity|Warning
|Resolution|Reset the management processor and reboot the server.

### iLO.iLOServicePortIsDisabled

**Description:**  The Service Port is disabled. Other Service Port properties cannot be changed.

|   |   |
|:---|:---|
|Message Format|"The Service Port is disabled. Other Service Port properties cannot be changed."
|Severity|Warning
|Resolution|Enable Service Port to modify other Service Port properties.

### HpeBiosMessageRegistry.MessagesMaxSizeExceeded

**Description:**  Indicates that the last configuration change attempted by the user resulted in a number of error messages that exceeded the maximum storage capacity alloted for messages corresponding to this resource.

|   |   |
|:---|:---|
|Message Format|"The messages array has been truncated because the last configuration change resulted in too many error messages."
|Severity|Warning
|Resolution|Inspect the last configuration change request for issues that may be generating errors, compare the request against the resource's schema, then retry the configuration change.

### HpeBiosMessageRegistry.UnsupportedAMPConfiguration

**Description:**  Indicates that the user provided Advanced Memory Protection (AMP) option is not appropriate for this memory configuration, as the underlying hardware does not support it.

|   |   |
|:---|:---|
|Message Format|"Underlying hardware does not support the requested AMP configuration, the settings are invalid."
|Severity|Warning
|Resolution|Ensure that the current memory configuration meets the requirements of the requested value before applying the settings.

### HpeBiosMessageRegistry.UnsupportedDramRaplValue

**Description:**  Indicates that the user provided Running Average Power Limit (RAPL) value could not be applied due to inherent DRAM power limitation. The value may be out of bounds or invalid.

|   |   |
|:---|:---|
|Message Format|"Underlying DRAM does not support the requested value."
|Severity|Warning
|Resolution|Ensure that the requested value is within the supported bounds before applying the settings.

### HpeBiosMessageRegistry.UnsupportedProcessorRaplValue

**Description:**  Indicates that the user provided Running Average Power Limit (RAPL) value could not be applied due to inherent processor power limitation. The value may be out of bounds or invalid.

|   |   |
|:---|:---|
|Message Format|"Underlying processor does not support the requested value."
|Severity|Warning
|Resolution|Ensure that the processor supports the requested value and that it is within the supported bounds before applying the settings.

