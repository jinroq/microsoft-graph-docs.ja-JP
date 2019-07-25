---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 7d617a5942f10a76bc1aa4b3d8b32864fbae661d
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35855578"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Report report = graphClient.reports()
    .getTeamsDeviceUsageUserDetail('D7')
    .buildRequest()
    .get();

```