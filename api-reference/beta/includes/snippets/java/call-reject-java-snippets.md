---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 797fc17308073d73333099f9a2d106658a237eb2
ms.sourcegitcommit: 56c0b609dfb1bc5d900956f407d107cdab7086e8
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/30/2019
ms.locfileid: "35933974"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

RejectReason reason = RejectReason.NONE;

graphClient.app().calls("{id}")
    .reject(reason,callbackUri)
    .buildRequest()
    .post();

```