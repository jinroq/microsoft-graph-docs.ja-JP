---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 419c07e5607de54b619bc22b504945ffa0fadcca
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35861972"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.domains("contoso.com")
    .buildRequest()
    .delete();

```