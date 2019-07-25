---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 517ca7495d78353ed70eb0b6a4f2175f93eb4fdb
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35724940"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var synchronizationSchema = new SynchronizationSchema
{
    Directories = new List<DirectoryDefinition>()
    {
        new DirectoryDefinition
        {
            Name = "Azure Active Directory",
            Objects = new List<ObjectDefinition>()
            {
                new ObjectDefinition
                {
                    Name = "User",
                    Attributes = new List<AttributeDefinition>()
                    {
                        new AttributeDefinition
                        {
                            Name = "userPrincipalName",
                            Type = AttributeType.String
                        }
                    }
                }
            }
        },
        new DirectoryDefinition
        {
            Name = "Salesforce"
        }
    },
    SynchronizationRules = new List<SynchronizationRule>()
    {
        new SynchronizationRule
        {
            Name = "USER_TO_USER",
            SourceDirectoryName = "Azure Active Directory",
            TargetDirectoryName = "Salesforce",
            ObjectMappings = new List<ObjectMapping>()
            {
                new ObjectMapping
                {
                    SourceObjectName = "User",
                    TargetObjectName = "User",
                    AttributeMappings = new List<AttributeMapping>()
                    {
                        new AttributeMapping
                        {
                            Source = new AttributeMappingSource
                            {
                            },
                            TargetAttributeName = "userName"
                        }
                    }
                }
            }
        }
    }
};

await graphClient.ServicePrincipals["{id}"].Synchronization.Jobs["{jobId}"].Schema
    .Request()
    .PutAsync(synchronizationSchema);

```