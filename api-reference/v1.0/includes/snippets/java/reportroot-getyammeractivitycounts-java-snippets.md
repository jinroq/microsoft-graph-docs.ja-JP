---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 530063dbaf9b9ddc1cc54482888f9c33414cb23f
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36320402"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Report report = graphClient.reports()
    .getYammerActivityCounts("D7")
    .buildRequest()
    .get();

```