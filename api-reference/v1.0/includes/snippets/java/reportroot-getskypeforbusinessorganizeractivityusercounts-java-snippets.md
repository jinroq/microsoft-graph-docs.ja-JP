---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 2662937b7b019496b96a42eab9def872581448aa
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35892335"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Report report = graphClient.reports()
    .getSkypeForBusinessOrganizerActivityUserCounts('D7')
    .buildRequest()
    .get();

```