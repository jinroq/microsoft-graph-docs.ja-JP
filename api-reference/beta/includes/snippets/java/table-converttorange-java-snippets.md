---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 9bbb9b264514b560ece8fd3634fffa60f1b5dfa9
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35869006"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().drive().items("{id}").workbook().tables("{id|name}")
    .convertToRange()
    .buildRequest()
    .post();

```