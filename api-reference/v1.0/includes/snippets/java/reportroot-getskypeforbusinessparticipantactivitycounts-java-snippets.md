---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 32f742195c0885e350cd58ed80884903639b3b0c
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36320718"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Report report = graphClient.reports()
    .getSkypeForBusinessParticipantActivityCounts("D7")
    .buildRequest()
    .get();

```