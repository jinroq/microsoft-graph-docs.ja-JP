---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 23e93cc7e46a9983cf1bdfcd2161c1107cf2c98b
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36320604"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Report report = graphClient.reports()
    .getSkypeForBusinessPeerToPeerActivityMinuteCounts("D7")
    .buildRequest()
    .get();

```