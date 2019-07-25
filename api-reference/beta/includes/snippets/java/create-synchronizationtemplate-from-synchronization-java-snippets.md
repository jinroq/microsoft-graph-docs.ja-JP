---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 4e69bf84380093c3c8acf041ee63841a1831a8e6
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35869082"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

SynchronizationTemplate synchronizationTemplate = new SynchronizationTemplate();
synchronizationTemplate.id = "SCIM-Test1";
synchronizationTemplate.applicationId = "{id}";
synchronizationTemplate.factoryTag = "CustomSCIM";

graphClient.applications("{id}").synchronization().templates()
    .buildRequest()
    .post(synchronizationTemplate);

```