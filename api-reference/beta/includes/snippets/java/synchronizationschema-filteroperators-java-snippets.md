---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: f2f92a824fe57658c4a4e6e7e69e9a43cd289c9e
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35869220"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IFilterOperatorSchemaCollectionPage filterOperators = graphClient.servicePrincipals("{id}").synchronization().jobs("{jobId}").schema()
    .filterOperators()
    .buildRequest()
    .get();

```