---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: f1795572ecdfa9e185dee24715a9ec89945fb13a
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35706326"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var verificationDnsRecords = await graphClient.Domains["contoso.com"].VerificationDnsRecords
    .Request()
    .GetAsync();

```