---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 019ee3f0cea10e8365eec845705b68b669902e2b
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36358440"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IYammerDeviceUsageUserDetailCollectionPage getYammerDeviceUsageUserDetail = graphClient.reports()
    .getYammerDeviceUsageUserDetail("D7")
    .buildRequest()
    .get();

```