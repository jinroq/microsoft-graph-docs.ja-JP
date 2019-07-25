---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 8a702590f9170d4184cc7c0014cb1854c62324b4
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35858476"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IEventCollectionPage events = graphClient.groups("{id}").events()
    .buildRequest()
    .get();

```