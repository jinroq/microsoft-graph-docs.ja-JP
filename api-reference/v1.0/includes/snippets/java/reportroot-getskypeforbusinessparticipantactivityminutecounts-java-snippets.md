---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: fad56a3f14cecfdf9e92b07c9341867465d60c07
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36320671"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Report report = graphClient.reports()
    .getSkypeForBusinessParticipantActivityMinuteCounts("D7")
    .buildRequest()
    .get();

```