---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 7ab1480a891989b10b8f4050e900013982ec2e5c
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36349266"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Report report = graphClient.reports()
    .getSkypeForBusinessActivityUserCounts("D7")
    .buildRequest()
    .get();

```