---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 09064bac41c0ae3c2f0a3ced1bb140b26edef22e
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36358738"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ITeamsUserActivityUserDetailCollectionPage getTeamsUserActivityUserDetail = graphClient.reports()
    .getTeamsUserActivityUserDetail("D7")
    .buildRequest()
    .get();

```