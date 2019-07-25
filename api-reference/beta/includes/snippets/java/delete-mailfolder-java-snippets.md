---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 11888dc38350d4272d7ecf6ef2a025fa3a303cb0
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35880150"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().mailFolders("AAMkAGVmMDEzM")
    .buildRequest()
    .delete();

```