---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 45b0dcf10d912945d996acb833a6ab6621f309fb
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35869459"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ISubscriptionCollectionPage subscriptions = graphClient.subscriptions()
    .buildRequest()
    .get();

```