---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 411d997ea542d53bf56e4674b5d0cb0df78f011a
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35880676"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String destinationId = "destinationId-value";

graphClient.me().messages("{id}")
    .copy(destinationId)
    .buildRequest()
    .post();

```