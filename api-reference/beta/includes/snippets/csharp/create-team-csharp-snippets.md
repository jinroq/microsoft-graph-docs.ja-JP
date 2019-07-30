---
description: 自動生成されたファイル。 変更しないでください
ms.openlocfilehash: dc995368988ac4493f306a5422994c4190feff33
ms.sourcegitcommit: 56c0b609dfb1bc5d900956f407d107cdab7086e8
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/30/2019
ms.locfileid: "35931947"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var team = new Team
{
    MemberSettings = new TeamMemberSettings
    {
        AllowCreateUpdateChannels = true
    },
    MessagingSettings = new TeamMessagingSettings
    {
        AllowUserEditMessages = true,
        AllowUserDeleteMessages = true
    },
    FunSettings = new TeamFunSettings
    {
        AllowGiphy = true,
        GiphyContentRating = GiphyRatingType.Strict
    },
    DiscoverySettings = new TeamDiscoverySettings
    {
        ShowInTeamsSearchAndSuggestions = true
    }
};

await graphClient.Groups["{id}"].Team
    .Request()
    .PutAsync(team);

```