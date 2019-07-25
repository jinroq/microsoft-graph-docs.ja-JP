---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 5b0c0236a8d9442c2af7f63d363d02779c9cdb53
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35877378"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

OutlookTaskGroup outlookTaskGroup = new OutlookTaskGroup();
outlookTaskGroup.name = "Leisure tasks";

graphClient.me().outlook().taskGroups()
    .buildRequest()
    .post(outlookTaskGroup);

```