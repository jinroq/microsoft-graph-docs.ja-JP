---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: cfda948bf615e89610f1d1db5ed2daf54ed5cacc
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35527292"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var supportedTimeZones = await graphClient.Me.Outlook.SupportedTimeZones(microsoft.graph.timeZoneStandard'Iana')
    .Request()
    .GetAsync();

```