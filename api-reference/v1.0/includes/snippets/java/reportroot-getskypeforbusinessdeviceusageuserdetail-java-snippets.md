---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 4bde10e0dc0a663300cc8c188818681c4c2ad797
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36349234"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Report report = graphClient.reports()
    .getSkypeForBusinessDeviceUsageUserDetail("D7")
    .buildRequest()
    .get();

```