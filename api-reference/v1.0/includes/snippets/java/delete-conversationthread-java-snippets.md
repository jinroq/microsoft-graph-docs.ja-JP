---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 3877fb170fd18433193436551df6c41962b770aa
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35883658"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.groups("{id}").threads("{id}")
    .buildRequest()
    .delete();

```