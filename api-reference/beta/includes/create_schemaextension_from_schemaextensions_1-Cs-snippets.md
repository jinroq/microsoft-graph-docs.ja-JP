---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: b28495a8098af8032ab4fcdae6a5029bdd6dca2f
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34439723"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var schemaExtension = new SchemaExtension
{
    Id = "graphlearn_courses",
    Description = "Graph Learn training courses extensions",
    TargetTypes = new List<String>()
    {
        "Group"
    },
    Properties = new List<ExtensionSchemaProperty>()
    {
        new ExtensionSchemaProperty
        {
            Name = "courseId",
            Type = "Integer"
        },
        new ExtensionSchemaProperty
        {
            Name = "courseName",
            Type = "String"
        },
        new ExtensionSchemaProperty
        {
            Name = "courseType",
            Type = "String"
        }
    }
};

await graphClient.SchemaExtensions
    .Request()
    .AddAsync(schemaExtension);

```