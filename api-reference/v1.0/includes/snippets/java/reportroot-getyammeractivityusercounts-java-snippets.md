---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 4265558c603e542ee4bc3b23fe4935b08b7ffb89
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36320363"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Report report = graphClient.reports()
    .getYammerActivityUserCounts("D7")
    .buildRequest()
    .get();

```