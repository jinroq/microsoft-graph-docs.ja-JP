---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 62168004d4ed49aaa44f1d7db181c953bc1cfa61
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35861583"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IDriveItemCollectionPage following = graphClient.me().drive().following()
    .buildRequest()
    .get();

```