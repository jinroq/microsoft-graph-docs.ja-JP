---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 3e5962e100c946161e53141e00a5d8c32e4d1277
ms.sourcegitcommit: 56c0b609dfb1bc5d900956f407d107cdab7086e8
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/30/2019
ms.locfileid: "35933956"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AudioRoutingGroup audioRoutingGroup = graphClient.app().calls("{id}").audioRoutingGroups("{id}")
    .buildRequest()
    .get();

```