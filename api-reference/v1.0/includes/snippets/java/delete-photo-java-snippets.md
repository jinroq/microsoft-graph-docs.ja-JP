---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: ba07150a6be3c77e035afb26a176a31980293891
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35855111"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.users("{id|userPrincipalName}").photo()
    .buildRequest()
    .delete();

```