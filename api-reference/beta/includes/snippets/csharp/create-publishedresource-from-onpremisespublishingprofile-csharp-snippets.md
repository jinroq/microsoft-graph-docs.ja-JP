---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: cbb431c9bca98cc811571c444c1b045aa0c62f5f
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35875039"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var publishedResource = new PublishedResource
{
    DisplayName = "New provisioning",
    ResourceName = "domain1.contoso.com"
};

await graphClient.OnPremisesPublishingProfiles["provisioning"].PublishedResources
    .Request()
    .AddAsync(publishedResource);

```