---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: b3dfa109dbf1e9c790869da2209f0b1465df7f1c
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36320430"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Report report = graphClient.reports()
    .getTeamsUserActivityUserCounts("D7")
    .buildRequest()
    .get();

```