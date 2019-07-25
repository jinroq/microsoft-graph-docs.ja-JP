---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: a367c1dd444aa9b74e85f5047c9510a473095401
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35883001"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Report report = graphClient.reports()
    .getYammerActivityCounts('D7')
    .buildRequest()
    .get();

```