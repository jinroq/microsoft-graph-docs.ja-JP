---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: fad918194947b5bf77743cf84d9ca052bc85ed51
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35869097"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ISynchronizationTemplateCollectionPage templates = graphClient.servicePrincipals("{id}").synchronization().templates()
    .buildRequest()
    .get();

```