---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 50954e9f2abbb5fee3a3f947f16bc894bb9c4cfb
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35736291"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var domain = new Domain
{
    IsDefault = true,
    SupportedServices = new List<String>()
    {
        "Email",
        "OfficeCommunicationsOnline"
    }
};

await graphClient.Domains["contoso.com"]
    .Request()
    .UpdateAsync(domain);

```