---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 1e9d6e6b3a9eeb355f8237bc36f2e8271d4ab226
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36359269"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ISkypeForBusinessOrganizerActivityMinuteCountsCollectionPage getSkypeForBusinessOrganizerActivityMinuteCounts = graphClient.reports()
    .getSkypeForBusinessOrganizerActivityMinuteCounts("D7")
    .buildRequest()
    .get();

```