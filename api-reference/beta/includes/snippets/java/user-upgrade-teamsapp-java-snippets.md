---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 98d1975a60511cc13e433d323157a9f8a1b4a131
ms.sourcegitcommit: 56c0b609dfb1bc5d900956f407d107cdab7086e8
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/30/2019
ms.locfileid: "35931213"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.users("{id}").teamwork().installedApps("{id}")
    .upgrade()
    .buildRequest()
    .post();

```