---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 611400aa968b86b6a733d4d5e453f2f1ea044fd5
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35889734"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().drive().items("{id}").workbook().tables("{id|name}")
    .headerRowRange()
    .buildRequest()
    .post();

```