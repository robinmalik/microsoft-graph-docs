---
description: "Automatically generated file. DO NOT MODIFY"
---

```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ExternalItem externalItem = new ExternalItem();
LinkedList<Acl> aclList = new LinkedList<Acl>();
Acl acl = new Acl();
acl.type = AclType.EVERYONE;
acl.value = "67a141d8-cf4e-4528-ba07-bed21bfacd2d";
acl.accessType = AccessType.GRANT;
acl.identitySource = IdentitySourceType.AZURE_ACTIVE_DIRECTORY;
aclList.add(acl);
externalItem.acl = aclList;

graphClient.external().connections("contosohr").items("TSP228082938")
	.buildRequest()
	.patch(externalItem);

```