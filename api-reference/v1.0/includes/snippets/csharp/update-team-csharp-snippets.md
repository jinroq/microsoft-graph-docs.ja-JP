---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 3488a2dd545cb9ec6f8e80604b9830779c3e6388
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35739725"
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
    }
};

await graphClient.Teams["{id}"]
    .Request()
    .UpdateAsync(team);

```