---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 6420978037c58731a0801e8ba5ba6cb253c200a1
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35864266"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String startCell = "startCell-value";

String endCell = "endCell-value";

graphClient.me().drive().items("{id}").workbook().worksheets("{id|name}").charts("{name}")
    .setPosition(startCell,endCell)
    .buildRequest()
    .post();

```