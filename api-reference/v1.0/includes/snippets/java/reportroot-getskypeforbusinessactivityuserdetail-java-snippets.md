---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 97c6a8d4750833fea54d898238e59ad41bc45dc2
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36349231"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Report report = graphClient.reports()
    .getSkypeForBusinessActivityUserDetail("D7")
    .buildRequest()
    .get();

```