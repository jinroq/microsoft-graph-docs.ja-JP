---
description: 自動生成されたファイル。 変更しないでください
ms.openlocfilehash: bb1c30f57a81630e40138e042c4fafcfd55ab204
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35888901"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IDirectoryObjectCollectionPage directReports = graphClient.me().directReports()
    .buildRequest()
    .get();

```