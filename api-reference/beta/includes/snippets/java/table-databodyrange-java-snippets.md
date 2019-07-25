---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: e13317d71cd9de797140784980ad2e44e2d8462a
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35868991"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().drive().items("{id}").workbook().tables("{id|name}")
    .dataBodyRange()
    .buildRequest()
    .post();

```