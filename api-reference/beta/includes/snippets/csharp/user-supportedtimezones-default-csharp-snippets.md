---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 2560ec005d7be76aa9be823be7dd6952c37b1df4
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35877279"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var supportedTimeZones = await graphClient.Me.Outlook
    .SupportedTimeZones()
    .Request()
    .GetAsync();

```