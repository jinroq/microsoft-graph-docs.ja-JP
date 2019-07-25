---
description: 自動生成されたファイル。 変更しないでください
ms.openlocfilehash: a94a3afcf2b9c6ed27e53d225a2718854e59b4fc
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35893843"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IMailFolderCollectionPage mailFolders = graphClient.me().mailFolders()
    .buildRequest()
    .get();

```