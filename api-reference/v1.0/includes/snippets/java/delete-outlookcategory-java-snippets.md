---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 8324d84c27fa47e08473fcaafa6866f5f8f02818
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35890578"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().outlook().masterCategories("4b1c2495-54c9-4a5e-90a2-0ab0b31987d8")
    .buildRequest()
    .delete();

```