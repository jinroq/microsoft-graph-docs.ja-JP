---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 0c999e559a954018abc044082ece5908601c0b67
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35877468"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IOutlookTaskFolderCollectionPage taskFolders = graphClient.me().outlook().taskFolders()
    .buildRequest()
    .get();

```