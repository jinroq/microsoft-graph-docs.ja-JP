---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 87903e4be5c2fda2cbc08df495717eaffc471f79
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35893818"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Report report = graphClient.reports()
    .getOffice365GroupsActivityStorage('D7')
    .buildRequest()
    .get();

```