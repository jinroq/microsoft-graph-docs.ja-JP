---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: d03078d9e828ffdff7df013b071893a946a6fa97
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35889825"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

boolean persistChanges = True;

graphClient.me().drive().items("{id}").workbook()
    .createSession(this,persistChanges)
    .buildRequest()
    .post();

```