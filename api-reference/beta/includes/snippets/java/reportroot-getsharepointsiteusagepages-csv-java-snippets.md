---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 048800bc87f5dbbb2bf21a7e1f4a334fae58b4c5
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35872593"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ISharePointSiteUsagePagesCollectionPage getSharePointSiteUsagePages = graphClient.reports()
    .getSharePointSiteUsagePages('D7')
    .buildRequest()
    .get();

```