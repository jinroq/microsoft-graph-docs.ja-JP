---
description: 自動生成されたファイル。 変更しないでください
ms.openlocfilehash: 39ad26cf2f5f79991e8c4a45dd8ccba8a3b2a94c
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35858155"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Group group = new Group();
group.description = "Self help community for golf";
group.displayName = "Golf Assist";
LinkedList<String> groupTypesList = new LinkedList<String>();
groupTypesList.add("Unified");
group.groupTypes = groupTypesList;
group.mailEnabled = true;
group.mailNickname = "golfassist";
group.securityEnabled = false;

graphClient.groups()
    .buildRequest()
    .post(group);

```