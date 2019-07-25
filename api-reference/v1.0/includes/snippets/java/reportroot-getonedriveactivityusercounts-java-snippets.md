---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: ccc176070b53421392e24b13395244993cb78929
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35893774"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Report report = graphClient.reports()
    .getOneDriveActivityUserCounts('D7')
    .buildRequest()
    .get();

```