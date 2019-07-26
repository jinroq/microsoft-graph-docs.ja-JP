---
description: 自動生成されたファイル。 変更しないでください
ms.openlocfilehash: ec341925c5adaed5e1a48e1ae5bc269a5ed90f94
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35885503"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ISiteCollectionPage sites = graphClient.sites("{site-id}").sites()
    .buildRequest()
    .get();

```