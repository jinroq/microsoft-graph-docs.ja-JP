---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 12e1700b69d9eff89422dfca1c6e36d5d2a0743e
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36349310"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Report report = graphClient.reports()
    .getSkypeForBusinessOrganizerActivityCounts("D7")
    .buildRequest()
    .get();

```