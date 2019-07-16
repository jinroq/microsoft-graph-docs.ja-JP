---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: ece37c53f1e271cbc48d0d4a46535b26b08144a2
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35738557"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var organization = new Organization
{
    MarketingNotificationEmails = new List<String>()
    {
        "marketing@contoso.com"
    },
    PrivacyProfile = new PrivacyProfile
    {
        ContactEmail = "alice@contoso.com",
        StatementUrl = "https://contoso.com/privacyStatement"
    },
    SecurityComplianceNotificationMails = new List<String>()
    {
        "security@contoso.com"
    },
    SecurityComplianceNotificationPhones = new List<String>()
    {
        "(123) 456-7890"
    },
    TechnicalNotificationMails = new List<String>()
    {
        "tech@contoso.com"
    }
};

await graphClient.Organization["{id}"]
    .Request()
    .UpdateAsync(organization);

```