---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 66a9dc75f0eb56bf94512594440b6834e6ab4c1d
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35884560"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IListItemVersionCollectionPage versions = graphClient.sites("{site-id}").lists("{list-id}").items("{item-id}").versions()
    .buildRequest()
    .get();

```