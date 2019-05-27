---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 5a963d8fc869aacfde5ff9d1bc390dd11acec3f6
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34463708"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var message = new Message
{
    Subject = "subject-value",
    Body = new ItemBody
    {
        ContentType = BodyType.Text,
        Content = "content-value"
    },
    InferenceClassification = InferenceClassificationType.Other
};

await graphClient.Me.Messages["{id}"]
    .Request()
    .UpdateAsync(message);

```