---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 10794a0931f365e128b99445b0744477a0549a10
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35869545"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ISubscribedSkuCollectionPage subscribedSkus = graphClient.subscribedSkus()
    .buildRequest()
    .get();

```