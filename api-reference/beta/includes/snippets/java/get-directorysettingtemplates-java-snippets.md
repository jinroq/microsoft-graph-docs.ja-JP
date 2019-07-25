---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: bae0bdc7527ba559fba969e1575ee48731e2508b
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35861991"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IDirectorySettingTemplateCollectionPage directorySettingTemplates = graphClient.directorySettingTemplates()
    .buildRequest()
    .get();

```