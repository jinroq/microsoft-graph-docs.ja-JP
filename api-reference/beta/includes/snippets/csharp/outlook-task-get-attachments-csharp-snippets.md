---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 95f9482afdb4efb55b847f63fb91815ed7770fe8
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35877706"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var attachments = await graphClient.Users["{id}"].Outlook.Tasks["{id}"].Attachments
    .Request()
    .GetAsync();

```