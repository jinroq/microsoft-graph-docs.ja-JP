---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 0e71b0f6bb162677608a636fb4a96ad4319f7a87
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36327461"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Report report = graphClient.reports()
    .getEmailActivityCounts("D7")
    .buildRequest()
    .get();

```