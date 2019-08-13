---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 867e064171878a2d487b41e743dbca169822abcd
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36321843"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Report report = graphClient.reports()
    .getSharePointActivityUserCounts("D7")
    .buildRequest()
    .get();

```