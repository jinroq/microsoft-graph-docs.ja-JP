---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 8bc8cfd763b32fd9e47d64409a053aea96bc57f0
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35868728"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().drive().items("{id}").workbook().tables("{id|name}").columns("{id|name}")
    .dataBodyRange()
    .buildRequest()
    .post();

```