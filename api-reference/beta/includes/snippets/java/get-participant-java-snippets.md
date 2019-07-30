---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 5303a252315697a99f053d41f2e1b1709859f7f8
ms.sourcegitcommit: 56c0b609dfb1bc5d900956f407d107cdab7086e8
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/30/2019
ms.locfileid: "35934001"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Participant participant = graphClient.app().calls("{id}").participants("{id}")
    .buildRequest()
    .get();

```