---
title: "Enum values"
description: "Microsoft Graph enumeration values"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
ms.localizationpriority: medium
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: enumTypes
---

### attributeFlowBehavior values 



|Member|
|:---|
|FlowWhenChanged|
|FlowAlways|

### attributeFlowType values 



|Member|
|:---|
|Always|
|ObjectAddOnly|
|MultiValueAddOnly|
|ValueAddOnly|
|AttributeAddOnly|

### attributeMappingSourceType values 



|Member|
|:---|
|Attribute|
|Constant|
|Function|

### attributeType values 



|Member|
|:---|
|String|
|Integer|
|Reference|
|Binary|
|Boolean|
|DateTime|

### directoryDefinitionDiscoverabilities values 



|Member|
|:---|
|None|
|AttributeNames|
|AttributeDataTypes|
|AttributeReadOnly|
|ReferenceAttributes|
|UnknownFutureValue|

### entryExportStatus values 



|Member|
|:---|
|Noop|
|Success|
|RetryableError|
|PermanentError|
|Error|

### entrySyncOperation values 



|Member|
|:---|
|None|
|Add|
|Delete|
|Update|

### mutability values 



|Member|
|:---|
|ReadWrite|
|ReadOnly|
|Immutable|
|WriteOnly|

### objectFlowTypes values 



|Member|
|:---|
|None|
|Add|
|Update|
|Delete|

### quarantineReason values 



|Member|
|:---|
|EncounteredBaseEscrowThreshold|
|EncounteredTotalEscrowThreshold|
|EncounteredEscrowProportionThreshold|
|EncounteredQuarantineException|
|Unknown|
|QuarantinedOnDemand|
|TooManyDeletes|
|IngestionInterrupted|

### scopeOperatorMultiValuedComparisonType values 



|Member|
|:---|
|All|
|Any|

### scopeOperatorType values 



|Member|
|:---|
|Binary|
|Unary|

### synchronizationJobRestartScope values 



|Member|
|:---|
|None|
|ConnectorDataStore|
|Escrows|
|Watermark|
|QuarantineState|
|Full|
|ForceDeletes|

### synchronizationScheduleState values 



|Member|
|:---|
|Active|
|Disabled|
|Paused|

### synchronizationSecret values 



|Member|
|:---|
|None|
|UserName|
|Password|
|SecretToken|
|AppKey|
|BaseAddress|
|ClientIdentifier|
|ClientSecret|
|SingleSignOnType|
|Sandbox|
|Url|
|Domain|
|ConsumerKey|
|ConsumerSecret|
|TokenKey|
|TokenExpiration|
|Oauth2AccessToken|
|Oauth2AccessTokenCreationTime|
|Oauth2RefreshToken|
|SyncAll|
|InstanceName|
|Oauth2ClientId|
|Oauth2ClientSecret|
|CompanyId|
|UpdateKeyOnSoftDelete|
|SynchronizationSchedule|
|SystemOfRecord|
|SandboxName|
|EnforceDomain|
|SyncNotificationSettings|
|SkipOutOfScopeDeletions|
|Oauth2AuthorizationCode|
|Oauth2RedirectUri|
|ApplicationTemplateIdentifier|
|Oauth2TokenExchangeUri|
|Oauth2AuthorizationUri|
|AuthenticationType|
|Server|
|PerformInboundEntitlementGrants|
|HardDeletesEnabled|
|SyncAgentCompatibilityKey|
|SyncAgentADContainer|
|ValidateDomain|
|TestReferences|
|ConnectionString|

### synchronizationStatusCode values 



|Member|
|:---|
|NotConfigured|
|NotRun|
|Active|
|Paused|
|Quarantine|

### synchronizationTaskExecutionResult values 



|Member|
|:---|
|Succeeded|
|Failed|
|EntryLevelErrors|

