---
description: 自動生成されたファイル。 変更しないでください
ms.openlocfilehash: 251083bf08b2770c07191c0b66a8c25d92576f20
ms.sourcegitcommit: 56c0b609dfb1bc5d900956f407d107cdab7086e8
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/30/2019
ms.locfileid: "35932553"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Team team = new Team();
TeamMemberSettings memberSettings = new TeamMemberSettings();
memberSettings.allowCreateUpdateChannels = true;
team.memberSettings = memberSettings;
TeamMessagingSettings messagingSettings = new TeamMessagingSettings();
messagingSettings.allowUserEditMessages = true;
messagingSettings.allowUserDeleteMessages = true;
team.messagingSettings = messagingSettings;
TeamFunSettings funSettings = new TeamFunSettings();
funSettings.allowGiphy = true;
funSettings.giphyContentRating = GiphyRatingType.STRICT;
team.funSettings = funSettings;

graphClient.groups("{id}").team()
    .buildRequest()
    .put(team);

```