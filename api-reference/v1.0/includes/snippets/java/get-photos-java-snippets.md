---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 09ae3e1b99dd791b78de74cdb63ddd33d0a5f8a4
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35889047"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IProfilePhotoCollectionPage photos = graphClient.groups("{id}").photos()
    .buildRequest()
    .get();

```