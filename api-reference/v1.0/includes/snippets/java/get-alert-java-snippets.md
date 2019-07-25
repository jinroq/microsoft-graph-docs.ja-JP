---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: b3f8800a73f563fadcf9341349ddb4fa15fb97ca
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35882656"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Alert alert = graphClient.security().alerts("{alert_id}")
    .buildRequest()
    .get();

```