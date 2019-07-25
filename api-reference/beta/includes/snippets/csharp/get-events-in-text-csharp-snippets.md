---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 798b6e60c12bcfdab5349b1927c85bf1b5d9fb5c
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35716547"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var events = await graphClient.Me.Events
    .Request()
    .Header("Prefer","outlook.body-content-type=\"text\"")
    .Select( e => new {
             e.Subject,
             e.Body,
             e.BodyPreview 
             })
    .GetAsync();

```