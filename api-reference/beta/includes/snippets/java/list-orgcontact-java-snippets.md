---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: b68ec07f7b8dcac374a56c8313e2aae48eda8636
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35877854"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IOrgContactCollectionPage contacts = graphClient.contacts()
    .buildRequest()
    .get();

```