---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 87519f761953fb32a0f6ddb9e3fb9db6dd08a62f
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35876866"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Place place = graphClient.places("3162F1E1-C4C0-604B-51D8-91DA78989EB1")
    .buildRequest()
    .get();

```