---
description: 自動生成されたファイル。 変更しないでください
ms.openlocfilehash: 4d8d058d8dde653af6c979aac4a40cbf6d0ec6a2
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35894093"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IDriveCollectionPage drives = graphClient.me().drives()
    .buildRequest()
    .get();

```