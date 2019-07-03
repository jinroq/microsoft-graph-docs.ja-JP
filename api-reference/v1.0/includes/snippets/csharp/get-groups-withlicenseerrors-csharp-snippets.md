---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: b33a360bc41eafde3315a28142ee02bc776fbb29
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35513738"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var groups = await graphClient.Groups
    .Request()
    .Filter("hasMembersWithLicenseErrors+eq+true,")
    .Select( e => new {
             e.Id,
             e.DisplayName 
             })
    .GetAsync();

```