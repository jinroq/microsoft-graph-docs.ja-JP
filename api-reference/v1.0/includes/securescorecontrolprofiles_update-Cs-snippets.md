---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 87af03c3fae97ba3e40abd0c4d41f746e8ef266f
ms.sourcegitcommit: c0df90d66cb2072848d4bb0bf730c47a601b99ce
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/29/2019
ms.locfileid: "34546473"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var secureScoreControlProfile = new SecureScoreControlProfile
{
    AssignedTo = "",
    Comment = "control is reviewed",
    State = "Reviewed",
    VendorInformation = new SecurityVendorInformation
    {
        Provider = "SecureScore",
        ProviderVersion = null,
        SubProvider = null,
        Vendor = "Microsoft"
    }
};

await graphClient.Security.SecureScoreControlProfiles["NonOwnerAccess"]
    .Request()
    .UpdateAsync(secureScoreControlProfile);

```