---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 1446e5d6c64808efa333ce2a1a42e231cc7d27bd
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35861646"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Drive drive = graphClient.users("{idOrUserPrincipalName}").drive()
    .buildRequest()
    .get();

```