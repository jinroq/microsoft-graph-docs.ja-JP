---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 34aab3d1def0aba64b2dabbf8a079827fed43d2b
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35880309"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IListCollectionPage lists = graphClient.sites("{site-id}").lists()
    .buildRequest()
    .get();

```