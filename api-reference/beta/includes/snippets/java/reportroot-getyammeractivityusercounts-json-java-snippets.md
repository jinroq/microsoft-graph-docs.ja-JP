---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 78529d8c9a1915eb0373dcc49e25ccf6662ae44d
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36358646"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IYammerActivitySummaryCollectionPage getYammerActivityUserCounts = graphClient.reports()
    .getYammerActivityUserCounts("D7")
    .buildRequest()
    .get();

```