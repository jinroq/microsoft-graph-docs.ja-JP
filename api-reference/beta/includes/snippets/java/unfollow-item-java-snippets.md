---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 0cd13de733260d732d533968e3dfc67a72ec8932
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35860905"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().drive().following("{item-id}")
    .buildRequest()
    .delete();

```