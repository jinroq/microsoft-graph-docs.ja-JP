---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 4d2e578d1e89fd049d321bad6ee34f7e02373ce5
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35861512"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IDriveItemCollectionPage recent = graphClient.me().drive()
    .recent()
    .buildRequest()
    .get();

```