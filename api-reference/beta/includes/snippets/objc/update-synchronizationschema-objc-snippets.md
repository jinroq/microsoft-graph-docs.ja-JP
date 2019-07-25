---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 4ac872dc2388f9d497c09b954f4999d00cf64ab1
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35724939"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/servicePrincipals/{id}/synchronization/jobs/{jobId}/schema"]]];
[urlRequest setHTTPMethod:@"PUT"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphSynchronizationSchema *synchronizationSchema = [[MSGraphSynchronizationSchema alloc] init];
NSMutableArray *directoriesList = [[NSMutableArray alloc] init];
MSGraphDirectoryDefinition *directories = [[MSGraphDirectoryDefinition alloc] init];
[directories setName:@"Azure Active Directory"];
NSMutableArray *objectsList = [[NSMutableArray alloc] init];
MSGraphObjectDefinition *objects = [[MSGraphObjectDefinition alloc] init];
[objects setName:@"User"];
NSMutableArray *attributesList = [[NSMutableArray alloc] init];
MSGraphAttributeDefinition *attributes = [[MSGraphAttributeDefinition alloc] init];
[attributes setName:@"userPrincipalName"];
[attributes setType: [MSGraphAttributeType String]];
[attributesList addObject: attributes];
[objects setAttributes:attributesList];
[objectsList addObject: objects];
[directories setObjects:objectsList];
[directoriesList addObject: directories];
MSGraphDirectoryDefinition *directories = [[MSGraphDirectoryDefinition alloc] init];
[directories setName:@"Salesforce"];
[directoriesList addObject: directories];
[synchronizationSchema setDirectories:directoriesList];
NSMutableArray *synchronizationRulesList = [[NSMutableArray alloc] init];
MSGraphSynchronizationRule *synchronizationRules = [[MSGraphSynchronizationRule alloc] init];
[synchronizationRules setName:@"USER_TO_USER"];
[synchronizationRules setSourceDirectoryName:@"Azure Active Directory"];
[synchronizationRules setTargetDirectoryName:@"Salesforce"];
NSMutableArray *objectMappingsList = [[NSMutableArray alloc] init];
MSGraphObjectMapping *objectMappings = [[MSGraphObjectMapping alloc] init];
[objectMappings setSourceObjectName:@"User"];
[objectMappings setTargetObjectName:@"User"];
NSMutableArray *attributeMappingsList = [[NSMutableArray alloc] init];
MSGraphAttributeMapping *attributeMappings = [[MSGraphAttributeMapping alloc] init];
MSGraphAttributeMappingSource *source = [[MSGraphAttributeMappingSource alloc] init];
[attributeMappings setSource:source];
[attributeMappings setTargetAttributeName:@"userName"];
[attributeMappingsList addObject: attributeMappings];
[objectMappings setAttributeMappings:attributeMappingsList];
[objectMappingsList addObject: objectMappings];
[synchronizationRules setObjectMappings:objectMappingsList];
[synchronizationRulesList addObject: synchronizationRules];
[synchronizationSchema setSynchronizationRules:synchronizationRulesList];

NSError *error;
NSData *synchronizationSchemaData = [synchronizationSchema getSerializedDataWithError:&error];
[urlRequest setHTTPBody:synchronizationSchemaData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```