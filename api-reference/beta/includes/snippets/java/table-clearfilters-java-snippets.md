---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 7d7d403a4286dea8316b28d8b611844c4a5a803d
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35869039"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().drive().items("{id}").workbook().tables("{id|name}")
    .clearFilters()
    .buildRequest()
    .post();

```