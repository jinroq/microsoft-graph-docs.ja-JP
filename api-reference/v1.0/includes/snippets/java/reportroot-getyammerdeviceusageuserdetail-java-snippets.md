---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 442f2f5e70c6e07a5c1a986b9f97a311bc93fec0
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35889639"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Report report = graphClient.reports()
    .getYammerDeviceUsageUserDetail('D7')
    .buildRequest()
    .get();

```