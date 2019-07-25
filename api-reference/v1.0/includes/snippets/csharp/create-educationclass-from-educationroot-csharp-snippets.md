---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 17f2500e14b0cbf0f0a52804fdb573ebdd85c97b
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35711443"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var educationClass = new EducationClass
{
    Description = "Health Level 1",
    ClassCode = "Health 501",
    DisplayName = "Health 1",
    ExternalId = "11019",
    ExternalName = "Health Level 1",
    ExternalSource = EducationExternalSource.Sis,
    MailNickname = "fineartschool.net"
};

await graphClient.Education.Classes
    .Request()
    .AddAsync(educationClass);

```