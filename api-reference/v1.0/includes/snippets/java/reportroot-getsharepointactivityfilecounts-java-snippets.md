---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 6ef2b2dcfdcd3c4cd125e41b9132ebbd34c50116
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36321754"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Report report = graphClient.reports()
    .getSharePointActivityFileCounts("D7")
    .buildRequest()
    .get();

```