---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 213ce90d6913c9fcdfd2c429441099d04a4e1a61
ms.sourcegitcommit: 56c0b609dfb1bc5d900956f407d107cdab7086e8
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/30/2019
ms.locfileid: "35932513"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String displayName = "Myprefix_test_mysuffix";

String mailNickname = "Myprefix_test_mysuffix";

String onBehalfOfUserId = "onBehalfOfUserId-value";

graphClient.groups("{id}")
    .validateProperties(displayName,mailNickname,onBehalfOfUserId)
    .buildRequest()
    .post();

```