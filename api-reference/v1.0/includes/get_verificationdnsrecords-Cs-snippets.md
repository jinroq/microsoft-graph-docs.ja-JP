---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: b60eb9de0e26ffa436a8ac1183ce310b65c4dd21
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34478329"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var verificationDnsRecords = await graphClient.Domains["{domain-name}"].VerificationDnsRecords
    .Request()
    .GetAsync();

```