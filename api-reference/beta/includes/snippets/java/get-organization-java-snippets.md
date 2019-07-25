---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 5d1599d8ff023c870f771f927a43e4069b7412aa
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35878105"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IOrganizationCollectionPage organization = graphClient.organization()
    .buildRequest()
    .get();

```