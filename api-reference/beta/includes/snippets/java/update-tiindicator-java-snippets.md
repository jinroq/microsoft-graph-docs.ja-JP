---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 3d4be1d97c1e89b719ecacce2d49dfd302d94ad7
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35868179"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new HeaderOption("Prefer", "return=representation"));

TiIndicator tiIndicator = new TiIndicator();
tiIndicator.additionalInformation = "additionalInformation-after-update";
tiIndicator.confidence = 42;
tiIndicator.description = "description-after-update";

graphClient.security().tiIndicators("{id}")
    .buildRequest( requestOptions )
    .patch(tiIndicator);

```