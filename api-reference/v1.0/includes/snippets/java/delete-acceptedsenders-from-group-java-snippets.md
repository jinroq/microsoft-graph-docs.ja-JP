---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 2d538a69800f44ea137293f837761771526c493c
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35856517"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.groups("{id}").acceptedSenders().references()
    .buildRequest()
    .delete();

```