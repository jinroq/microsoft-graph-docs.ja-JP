---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 9ff82720fb7db5f024ae2076955f892a967e3951
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35880198"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

FieldValueSet fieldValueSet = new FieldValueSet();
fieldValueSet.Color = "Fuchsia";
fieldValueSet.Quantity = 934;

graphClient.sites("{site-id}").lists("{list-id}").items("{item-id}").fields()
    .buildRequest()
    .patch(fieldValueSet);

```