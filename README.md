# ![LOGO](logo.png) Google Cloud Memorystore for Redis **flow**ground Connector

## Description

A generated **flow**ground connector for the Google Cloud Memorystore for Redis API (version v1).

Generated from: https://api.apis.guru/v2/specs/googleapis.com/redis/v1/swagger.json<br/>
Generated at: 2019-05-07T17:41:53+03:00

## API Description

Creates and manages Redis instances on the Google Cloud Platform.

## Authorization

Supported authorization schemes:
- OAuth2

For OAuth 2.0 you need to specify OAuth Client credentials as environment variables in the connector repository:
* `OAUTH_CLIENT_ID` - your OAuth client id
* `OAUTH_CLIENT_SECRET` - your OAuth client secret

## Actions

### Deletes a specific Redis instance.  Instance stops serving and data is<br/>
> deleted.

*Tags:* `projects`

#### Input Parameters
* `name` - _required_ - Required. Redis instance resource name using the form:
    `projects/{project_id}/locations/{location_id}/instances/{instance_id}`
where `location_id` refers to a GCP region
* `access_token` - _optional_ - OAuth access token.
* `alt` - _optional_ - Data format for response.
    Possible values: json, media, proto.
* `callback` - _optional_ - JSONP
* `fields` - _optional_ - Selector specifying which fields to include in a partial response.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - Available to use for quota purposes for server-side applications. Can be any arbitrary string assigned to a user, but should not exceed 40 characters.
* `uploadType` - _optional_ - Legacy upload protocol for media (e.g. "media", "multipart").
* `upload_protocol` - _optional_ - Upload protocol for media (e.g. "raw", "multipart").

### Gets the details of a specific Redis instance.

*Tags:* `projects`

#### Input Parameters
* `name` - _required_ - Required. Redis instance resource name using the form:
    `projects/{project_id}/locations/{location_id}/instances/{instance_id}`
where `location_id` refers to a GCP region
* `access_token` - _optional_ - OAuth access token.
* `alt` - _optional_ - Data format for response.
    Possible values: json, media, proto.
* `callback` - _optional_ - JSONP
* `fields` - _optional_ - Selector specifying which fields to include in a partial response.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - Available to use for quota purposes for server-side applications. Can be any arbitrary string assigned to a user, but should not exceed 40 characters.
* `uploadType` - _optional_ - Legacy upload protocol for media (e.g. "media", "multipart").
* `upload_protocol` - _optional_ - Upload protocol for media (e.g. "raw", "multipart").

### Updates the metadata and configuration of a specific Redis instance.<br/>
> <br/>
> Completed longrunning.Operation will contain the new instance object<br/>
> in the response field. The returned operation is automatically deleted<br/>
> after a few hours, so there is no need to call DeleteOperation.

*Tags:* `projects`

#### Input Parameters
* `name` - _required_ - Required. Unique name of the resource in this scope including project and
location using the form:
    `projects/{project_id}/locations/{location_id}/instances/{instance_id}`

Note: Redis instances are managed and addressed at regional level so
location_id here refers to a GCP region; however, users may choose which
specific zone (or collection of zones for cross-zone instances) an instance
should be provisioned in. Refer to [location_id] and
[alternative_location_id] fields for more details.
* `updateMask` - _optional_ - Required. Mask of fields to update. At least one path must be supplied in
this field. The elements of the repeated paths field may only include these
fields from Instance:

 *   `displayName`
 *   `labels`
 *   `memorySizeGb`
 *   `redisConfig`
* `alt` - _optional_ - Data format for response.
    Possible values: json, media, proto.
* `callback` - _optional_ - JSONP
* `fields` - _optional_ - Selector specifying which fields to include in a partial response.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - Available to use for quota purposes for server-side applications. Can be any arbitrary string assigned to a user, but should not exceed 40 characters.
* `uploadType` - _optional_ - Legacy upload protocol for media (e.g. "media", "multipart").
* `upload_protocol` - _optional_ - Upload protocol for media (e.g. "raw", "multipart").

### Lists information about the supported locations for this service.

*Tags:* `projects`

#### Input Parameters
* `filter` - _optional_ - The standard list filter.
* `name` - _required_ - The resource that owns the locations collection, if applicable.
* `pageSize` - _optional_ - The standard list page size.
* `pageToken` - _optional_ - The standard list page token.
* `fields` - _optional_ - Selector specifying which fields to include in a partial response.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - Available to use for quota purposes for server-side applications. Can be any arbitrary string assigned to a user, but should not exceed 40 characters.
* `uploadType` - _optional_ - Legacy upload protocol for media (e.g. "media", "multipart").
* `upload_protocol` - _optional_ - Upload protocol for media (e.g. "raw", "multipart").

### Lists operations that match the specified filter in the request. If the<br/>
> server doesn't support this method, it returns `UNIMPLEMENTED`.<br/>
> <br/>
> NOTE: the `name` binding allows API services to override the binding<br/>
> to use different resource name schemes, such as `users/*/operations`. To<br/>
> override the binding, API services can add a binding such as<br/>
> `"/v1/{name=users/*}/operations"` to their service configuration.<br/>
> For backwards compatibility, the default name includes the operations<br/>
> collection id, however overriding users must ensure the name binding<br/>
> is the parent resource, without the operations collection id.

*Tags:* `projects`

#### Input Parameters
* `filter` - _optional_ - The standard list filter.
* `name` - _required_ - The name of the operation's parent resource.
* `pageSize` - _optional_ - The standard list page size.
* `pageToken` - _optional_ - The standard list page token.
* `fields` - _optional_ - Selector specifying which fields to include in a partial response.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - Available to use for quota purposes for server-side applications. Can be any arbitrary string assigned to a user, but should not exceed 40 characters.
* `uploadType` - _optional_ - Legacy upload protocol for media (e.g. "media", "multipart").
* `upload_protocol` - _optional_ - Upload protocol for media (e.g. "raw", "multipart").

### Starts asynchronous cancellation on a long-running operation.  The server<br/>
> makes a best effort to cancel the operation, but success is not<br/>
> guaranteed.  If the server doesn't support this method, it returns<br/>
> `google.rpc.Code.UNIMPLEMENTED`.  Clients can use<br/>
> Operations.GetOperation or<br/>
> other methods to check whether the cancellation succeeded or whether the<br/>
> operation completed despite cancellation. On successful cancellation,<br/>
> the operation is not deleted; instead, it becomes an operation with<br/>
> an Operation.error value with a google.rpc.Status.code of 1,<br/>
> corresponding to `Code.CANCELLED`.

*Tags:* `projects`

#### Input Parameters
* `name` - _required_ - The name of the operation resource to be cancelled.
* `access_token` - _optional_ - OAuth access token.
* `alt` - _optional_ - Data format for response.
    Possible values: json, media, proto.
* `callback` - _optional_ - JSONP
* `fields` - _optional_ - Selector specifying which fields to include in a partial response.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - Available to use for quota purposes for server-side applications. Can be any arbitrary string assigned to a user, but should not exceed 40 characters.
* `uploadType` - _optional_ - Legacy upload protocol for media (e.g. "media", "multipart").
* `upload_protocol` - _optional_ - Upload protocol for media (e.g. "raw", "multipart").

### Lists all Redis instances owned by a project in either the specified<br/>
> location (region) or all locations.<br/>
> <br/>
> The location should have the following format:<br/>
> * `projects/{project_id}/locations/{location_id}`<br/>
> <br/>
> If `location_id` is specified as `-` (wildcard), then all regions<br/>
> available to the project are queried, and the results are aggregated.

*Tags:* `projects`

#### Input Parameters
* `pageSize` - _optional_ - The maximum number of items to return.

If not specified, a default value of 1000 will be used by the service.
Regardless of the page_size value, the response may include a partial list
and a caller should only rely on response's
next_page_token
to determine if there are more instances left to be queried.
* `pageToken` - _optional_ - The next_page_token value returned from a previous List request,
if any.
* `parent` - _required_ - Required. The resource name of the instance location using the form:
    `projects/{project_id}/locations/{location_id}`
where `location_id` refers to a GCP region
* `callback` - _optional_ - JSONP
* `fields` - _optional_ - Selector specifying which fields to include in a partial response.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - Available to use for quota purposes for server-side applications. Can be any arbitrary string assigned to a user, but should not exceed 40 characters.
* `uploadType` - _optional_ - Legacy upload protocol for media (e.g. "media", "multipart").
* `upload_protocol` - _optional_ - Upload protocol for media (e.g. "raw", "multipart").

### Creates a Redis instance based on the specified tier and memory size.<br/>
> <br/>
> By default, the instance is accessible from the project's<br/>
> [default network](/compute/docs/networks-and-firewalls#networks).<br/>
> <br/>
> The creation is executed asynchronously and callers may check the returned<br/>
> operation to track its progress. Once the operation is completed the Redis<br/>
> instance will be fully functional. Completed longrunning.Operation will<br/>
> contain the new instance object in the response field.<br/>
> <br/>
> The returned operation is automatically deleted after a few hours, so there<br/>
> is no need to call DeleteOperation.

*Tags:* `projects`

#### Input Parameters
* `instanceId` - _optional_ - Required. The logical name of the Redis instance in the customer project
with the following restrictions:

* Must contain only lowercase letters, numbers, and hyphens.
* Must start with a letter.
* Must be between 1-40 characters.
* Must end with a number or a letter.
* Must be unique within the customer project / location
* `parent` - _required_ - Required. The resource name of the instance location using the form:
    `projects/{project_id}/locations/{location_id}`
where `location_id` refers to a GCP region
* `alt` - _optional_ - Data format for response.
    Possible values: json, media, proto.
* `callback` - _optional_ - JSONP
* `fields` - _optional_ - Selector specifying which fields to include in a partial response.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - Available to use for quota purposes for server-side applications. Can be any arbitrary string assigned to a user, but should not exceed 40 characters.
* `uploadType` - _optional_ - Legacy upload protocol for media (e.g. "media", "multipart").
* `upload_protocol` - _optional_ - Upload protocol for media (e.g. "raw", "multipart").

## License

**flow**ground :- Telekom iPaaS / googleapis-com-redis-connector<br/>
Copyright © 2019, [Deutsche Telekom AG](https://www.telekom.de)<br/>
contact: flowground@telekom.de

All files of this connector are licensed under the Apache 2.0 License. For details
see the file LICENSE on the toplevel directory.
