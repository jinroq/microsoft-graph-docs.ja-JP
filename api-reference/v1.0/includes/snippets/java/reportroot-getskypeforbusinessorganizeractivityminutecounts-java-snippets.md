---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 4f0a8ab3648e3d5e0e3f9a37e9f3648157dca8a4
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36349224"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Report report = graphClient.reports()
    .getSkypeForBusinessOrganizerActivityMinuteCounts("D7")
    .buildRequest()
    .get();

```