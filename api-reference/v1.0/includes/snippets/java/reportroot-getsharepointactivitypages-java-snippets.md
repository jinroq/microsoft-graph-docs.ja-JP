---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: ab871cf8fa96b598a70bade68feac4869428abcb
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36321753"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Report report = graphClient.reports()
    .getSharePointActivityPages("D7")
    .buildRequest()
    .get();

```