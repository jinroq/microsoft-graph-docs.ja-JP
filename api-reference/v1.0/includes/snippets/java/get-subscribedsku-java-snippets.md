---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 645d281ef47479f4921a97515e7b2f2227f5a8e1
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35890595"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

SubscribedSku subscribedSku = graphClient.subscribedSkus("{id}")
    .buildRequest()
    .get();

```