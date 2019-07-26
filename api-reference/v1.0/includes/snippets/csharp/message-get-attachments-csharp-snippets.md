---
description: 自動生成されたファイル。 変更しないでください
ms.openlocfilehash: ff29bbad94daeb381a85f2507e65ef80eef93bf5
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35885030"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var attachments = await graphClient.Me.Messages["{id}"].Attachments
    .Request()
    .GetAsync();

```