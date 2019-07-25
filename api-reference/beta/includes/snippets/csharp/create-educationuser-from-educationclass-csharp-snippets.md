---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: c7d9e8b9ce9cbdc33f0ed1d8069c724ab8da875b
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35860544"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var educationUser = new EducationUser
{
    AdditionalData = new Dictionary<string, object>()
    {
        {"@odata.id","https://graph.microsoft.com/beta/education/users/14011"}
    }
};

await graphClient.Education.Classes["11017"].Teachers.References
    .Request()
    .AddAsync(educationUser);

```