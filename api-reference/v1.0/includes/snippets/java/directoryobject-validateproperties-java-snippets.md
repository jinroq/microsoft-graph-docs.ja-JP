---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 6262508001c3419c7b52326a375e836fae8f55d7
ms.sourcegitcommit: 56c0b609dfb1bc5d900956f407d107cdab7086e8
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/30/2019
ms.locfileid: "35932217"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String entityType = "Group";

String displayName = "Myprefix_test_mysuffix";

String mailNickname = "Myprefix_test_mysuffix";

String onBehalfOfUserId = "onBehalfOfUserId-value";

graphClient.directoryObjects()
    .validateProperties(entityType,displayName,mailNickname,onBehalfOfUserId)
    .buildRequest()
    .post();

```