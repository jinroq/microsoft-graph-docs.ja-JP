---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: b60eb9de0e26ffa436a8ac1183ce310b65c4dd21
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35513823"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var verificationDnsRecords = await graphClient.Domains["{domain-name}"].VerificationDnsRecords
    .Request()
    .GetAsync();

```