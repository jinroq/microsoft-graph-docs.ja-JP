---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: d719db2d94c9271c783a82155cf6547442df6270
ms.sourcegitcommit: 56c0b609dfb1bc5d900956f407d107cdab7086e8
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/30/2019
ms.locfileid: "35933998"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

OnlineMeeting onlineMeeting = graphClient.app().onlineMeetings("{id}")
    .buildRequest()
    .get();

```