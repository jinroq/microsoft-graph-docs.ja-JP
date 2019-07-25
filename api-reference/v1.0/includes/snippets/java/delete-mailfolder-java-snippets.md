---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 0727804d9b54e1dfb934744943da841d9bfbaf73
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35893122"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().mailFolders("{id}")
    .buildRequest()
    .delete();

```