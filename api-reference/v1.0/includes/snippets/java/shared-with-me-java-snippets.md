---
description: 自動生成されたファイル。 変更しないでください
ms.openlocfilehash: 139f0b81531af87133780d9d7177cf044198d7f8
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35883068"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IDriveItemCollectionPage sharedWithMe = graphClient.me().drive()
    .sharedWithMe()
    .buildRequest()
    .get();

```