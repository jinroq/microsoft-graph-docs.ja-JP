---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 5060610d40b31611b05e67c3558806421dafa5b5
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36320571"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Report report = graphClient.reports()
    .getSkypeForBusinessPeerToPeerActivityUserCounts("D7")
    .buildRequest()
    .get();

```