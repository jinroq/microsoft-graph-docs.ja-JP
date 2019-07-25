---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 37a75109ebd7bd79911364df2feb8a04f21464f8
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35873347"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IOffice365GroupsActivityDetailCollectionPage getOffice365GroupsActivityDetail = graphClient.reports()
    .getOffice365GroupsActivityDetail('D7')
    .buildRequest()
    .get();

```