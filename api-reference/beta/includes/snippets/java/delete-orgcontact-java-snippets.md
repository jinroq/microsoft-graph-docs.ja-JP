---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 45c54efc5004aab3c2877be2fc54f1c840282242
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35878079"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.contacts("{id}")
    .buildRequest()
    .delete();

```