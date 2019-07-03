---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: d81e85f91edd75ffa8d91c462f9e585b64d6f656
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35503738"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var attachment = await graphClient.Me.Messages["AAMkAGUzY5QKjAAA="].Attachments["AAMkAGUzY5QKjAAABEgAQAMkpJI_X-LBFgvrv1PlZYd8="]
    .Request()
    .GetAsync();

```