---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 54da9e3a28a5338a749698a79a5d8b8d610ce080
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35526086"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var attachment = new Attachment
{
    LastModifiedDateTime = "datetime-value",
    Name = "name-value",
    ContentType = "contentType-value",
    Size = 99,
    IsInline = true
};

await graphClient.Users["{id}"].Outlook.Tasks["{id}"].Attachments
    .Request()
    .AddAsync(attachment);

```