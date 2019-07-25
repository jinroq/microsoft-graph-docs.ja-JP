---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 879b2298b63ee9af2937259c0870441c7e6becf0
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35885902"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Report report = graphClient.reports()
    .getYammerDeviceUsageUserCounts('D7')
    .buildRequest()
    .get();

```