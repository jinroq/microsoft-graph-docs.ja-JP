---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 35a28ae0caaa32f2f4774c7f02a1cbefed7c3160
ms.sourcegitcommit: 56c0b609dfb1bc5d900956f407d107cdab7086e8
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/30/2019
ms.locfileid: "35931030"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.servicePrincipals("{id}").synchronization().jobs("{jobId}").schema().directories("{directoryId}")
    .discover()
    .buildRequest()
    .post();

```