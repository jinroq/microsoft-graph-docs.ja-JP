---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 8d2780d88f14407a751d16a599601f3df09c40b6
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35486356"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var schemaExtension = new SchemaExtension
{
    Properties = new List<ExtensionSchemaProperty>()
    {
        new ExtensionSchemaProperty
        {
            Name = "new-name-value",
            Type = "new-type-value"
        },
        new ExtensionSchemaProperty
        {
            Name = "additional-name-value",
            Type = "additional-type-value"
        }
    }
};

await graphClient.SchemaExtensions["{id}"]
    .Request()
    .UpdateAsync(schemaExtension);

```