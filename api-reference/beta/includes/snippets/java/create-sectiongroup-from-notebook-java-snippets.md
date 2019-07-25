---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 851021b071fe66cb8df8d090d8928714b6830c65
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35879018"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

SectionGroup sectionGroup = new SectionGroup();
sectionGroup.displayName = "Section group name";

graphClient.me().onenote().notebooks("{id}").sectionGroups()
    .buildRequest()
    .post(sectionGroup);

```