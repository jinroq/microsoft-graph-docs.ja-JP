---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: fc40a5815946e0180574b62231347dcf8916cf46
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36349338"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Report report = graphClient.reports()
    .getSkypeForBusinessActivityCounts("D7")
    .buildRequest()
    .get();

```