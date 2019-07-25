---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 0cf216dfc4ced8f1c65e04ea9b71da1d245b288e
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35714238"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var @event = await graphClient.Me.Events["AAMkAGI1AAAoZDOFAAA="]
    .Request()
    .Header("Prefer","outlook.body-content-type=\"text\"")
    .Select( e => new {
             e.Subject,
             e.Body,
             e.BodyPreview 
             })
    .GetAsync();

```