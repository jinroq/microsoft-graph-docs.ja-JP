---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 2626ebb2ba1a55f6c08f8b71386ca1e4927e5369
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35883481"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IDirectoryObjectCollectionPage memberOf = graphClient.devices("{id}").memberOf()
    .buildRequest()
    .get();

```