---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: f888a02ae45de3ab44b611ef2127f41ce5ae9018
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/15/2019
ms.locfileid: "36422244"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Group group = graphClient.education().classes("{class-id}").group()
    .buildRequest()
    .get();

```