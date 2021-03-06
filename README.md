# ![LOGO](logo.png) AuthorizationManagementClient **flow**ground Connector

## Description

A generated **flow**ground connector for the AuthorizationManagementClient API (version 2018-01-01-preview).

Generated from: https://api.apis.guru/v2/specs/azure.com/authorization-authorization-RoleDefinitionsCalls/2018-01-01-preview/swagger.json<br/>
Generated at: 2019-06-11T18:13:21+03:00

## API Description

Role based access control provides you a way to apply granular level policy administration down to individual resources or resource groups. These operations allow you to manage role definitions. A role definition describes the set of actions that can be performed on resources.

## Authorization

Supported authorization schemes:
- OAuth2

For OAuth 2.0 you need to specify OAuth Client credentials as environment variables in the connector repository:
* `OAUTH_CLIENT_ID` - your OAuth client id
* `OAUTH_CLIENT_SECRET` - your OAuth client secret

## Actions

### Gets all permissions the caller has for a resource group.

*Tags:* `Permissions`

#### Input Parameters
* `resourceGroupName` - _required_ - The name of the resource group.
* `api-version` - _required_ - The API version to use for this operation.
* `subscriptionId` - _required_ - The ID of the target subscription.

### Gets all permissions the caller has for a resource.

*Tags:* `Permissions`

#### Input Parameters
* `resourceGroupName` - _required_ - The name of the resource group.
* `resourceProviderNamespace` - _required_ - The namespace of the resource provider.
* `parentResourcePath` - _required_ - The parent resource identity.
* `resourceType` - _required_ - The resource type of the resource.
* `resourceName` - _required_ - The name of the resource to get the permissions for.
* `api-version` - _required_ - The API version to use for this operation.
* `subscriptionId` - _required_ - The ID of the target subscription.

### Get all role definitions that are applicable at scope and above.

*Tags:* `RoleDefinitions`

#### Input Parameters
* `scope` - _required_ - The scope of the role definition.
* `$filter` - _optional_ - The filter to apply on the operation. Use atScopeAndBelow filter to search below the given scope as well.
* `api-version` - _required_ - The API version to use for this operation.

### Deletes a role definition.

*Tags:* `RoleDefinitions`

#### Input Parameters
* `scope` - _required_ - The scope of the role definition.
* `roleDefinitionId` - _required_ - The ID of the role definition to delete.
* `api-version` - _required_ - The API version to use for this operation.

### Get role definition by name (GUID).

*Tags:* `RoleDefinitions`

#### Input Parameters
* `scope` - _required_ - The scope of the role definition.
* `roleDefinitionId` - _required_ - The ID of the role definition.
* `api-version` - _required_ - The API version to use for this operation.

### Creates or updates a role definition.

*Tags:* `RoleDefinitions`

#### Input Parameters
* `scope` - _required_ - The scope of the role definition.
* `roleDefinitionId` - _required_ - The ID of the role definition.
* `api-version` - _required_ - The API version to use for this operation.

## License

**flow**ground :- Telekom iPaaS / azure-com-authorization-authorization-role-definitions-calls-connector<br/>
Copyright © 2019, [Deutsche Telekom AG](https://www.telekom.de)<br/>
contact: flowground@telekom.de

All files of this connector are licensed under the Apache 2.0 License. For details
see the file LICENSE on the toplevel directory.
