---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: de478f68f0e67b20e5126a175129414c738cd565
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35873863"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IEmailAppUsageUserDetailCollectionPage getEmailAppUsageUserDetail = graphClient.reports()
    .getEmailAppUsageUserDetail('D7')
    .buildRequest()
    .get();

```