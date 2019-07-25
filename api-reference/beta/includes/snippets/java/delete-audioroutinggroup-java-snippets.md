---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 44858ef3107a52a70792eccbed9c9cbbc9c4c349
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35856980"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.app().calls("{id}").audioRoutingGroups("{id}")
    .buildRequest()
    .delete();

```